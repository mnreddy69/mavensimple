pipeline {
   agent any

   tools {
       maven "maven"
   }

   stages {
      stage('Build') {
         steps {
           sh "mvn -Dmaven.test.failure.ignore=true clean compile"
         }
         }
      stage("Test") {
          steps {
            sh "mvn -Dmaven.test.failure.ignore=true clean test"
            
          }

      }
      stage("Deploy") {
          steps {
            sh "mvn -Dmaven.test.failure.ignore=true clean install"
            
          }
        
              }

          }


      }

  
