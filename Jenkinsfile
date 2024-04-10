pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
      steps {
        sh 'docker build -t madhanmohanreddyeeda/mmr-46org-frontend .'
      }
    }

    stage('Docker Push') {
      steps {
        sh 'docker push madhanmohanreddyeeda/mmr-46org-frontend'
      }
    }

  }
}