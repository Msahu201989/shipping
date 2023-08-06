pipeline {

 agent {
    node { label 'Workstation' }
 }

 stages {

   stage ('compile code') {
     steps {
      echo 'compile code'
     }
   }

  stage ('code quality') {
    steps {
     echo 'code quality'
    }
  }

    stage ('Style checks') {
          steps {
       echo 'style checks'
      }
    }

      stage ('unit Tests') {
        steps {
         echo 'Unit Test'
        }
      }

      stage ('Build Packages') {
        steps {
         echo 'Download Dependencies'
        }
      }

       stage ('Prepare Artifact') {
         steps {
          echo 'Prepare Artifact'
         }
       }

         stage ('Publish Artifact') {
           steps {
            echo 'Publish Artifact'
           }
         }
 }
 }


