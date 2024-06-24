pipeline {
  agent {
    docker { image 'node:16-alpine' }
    // docker { image 'gcr.io/kaniko-project/executor --no-push' }
  }
  stages {
    stage('Test') {
      steps {
        sh 'ls -l'
      }
    }
  }
}