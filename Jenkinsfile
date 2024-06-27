pipeline {
  agent {
    // docker { image 'node:16-alpine' }
    docker { image 'gcr.io/kaniko-project/executor' }
  }
  stages {
    stage('docker build') {
      steps {
        sh 'docker build -t static-site --no-push .'
      }
    }
  }
}