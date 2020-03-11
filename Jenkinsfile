pipeline {
  agent any
  stages {
    stage('jdk-7') {
      parallel {
        stage('jdk-7') {
          agent any
          steps {
            sh 'echo "coming from jdk 7"'
          }
        }

        stage('jdk-8') {
          agent {
            node {
              label 'jdk-8'
            }

          }
          steps {
            sh 'echo "Coming from jdk-8"'
          }
        }

      }
    }

  }
}