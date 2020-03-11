pipeline {
  agent {
    docker {
      image 'nginx'
    }

  }
  stages {
    stage('mydocker') {
      steps {
        sh 'echo "hello from docker"'
      }
    }

  }
}