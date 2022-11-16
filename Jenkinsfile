pipeline {

 agent any

 stages {

  stage('compile code'){
   steps{
    echo 'compile code'
     sh 'env'
    }
   }

  stage('code Quality') {
   steps{
     echo 'code Quality'
     sh 'env'
     }
   }

   stage('Style Checks') {
     when {
       anyOf {
         branch 'main'
         tag "*"
        }
     }
    steps{
      echo 'style checks'
      }
    }

    stage('Unit Tests'){
      when {
          anyOf {
           branch 'main'
           tag "*"
           }
        }
     steps{
       echo 'code Quality'
       }
     }

    stage('Build Package') {
     when { tag "*" }
      steps {
        echo 'Download Dependencies'
        }
        }

    stage('Prepare Artifact') {
      when { tag "*" }
      steps {
        echo 'Prepare Artifact'
        }
        }

    stage('Publish Artifact') {
      when { tag "*" }
      steps {
        echo 'Publish Artifact'
        }
        }
    }
 }