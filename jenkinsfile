pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
      steps {
        sh 'docker build -t madhanmohanreddyeeda/MMR-46org-frontend .'
      }
    }

    stage('Docker Push') {
      steps {
        sh 'docker push madhanmohanreddyeeda/MMR-46org-frontend'
      }
    }

  }
}