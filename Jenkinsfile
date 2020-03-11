pipeline {
  agent any
  stages {
    stage('jdk-7') {
      parallel {
        stage('jdk-7') {
          agent any
          steps {
            sh 'echo "coming from jdk 7"'
            stash(name: 'Stash-file-7', includes: 'targets/**')
            unstash 'unstash-jdk7'
          }
        }

        stage('jdk-8') {
          agent any
          steps {
            sh 'echo "Coming from jdk-8"'
          }
        }

      }
    }

  }
}