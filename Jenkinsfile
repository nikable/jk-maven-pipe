pipeline {
    agent {label 'linux'}
    tools {
      maven 'maven-3.5.0'
    }
    stages {
        stage ('hello'){
           steps {
           script {
               echo "test"
            }

           }
        }

        stage ('maven build') {
          steps {
            sh 'mvn clean compile'

          }

        }

        stage ('maven package') {
          steps {
           sh 'mvn package'

          }

        }


    }
}