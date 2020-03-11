pipeline {
  agent any
  stages {
    stage('jdk-7') {
      parallel {
        stage('jdk-7') {
          steps {
            sh 'echo "coming from jdk 7"'
          }
        }

        stage('jdk-8') {
          steps {
            sh 'echo "Coming from jdk-8"'
          }
        }

      }
    }

  }
}