pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
      steps {
        sh 'docker build -t madhanmohanreddyeeda/github-repo-frontend .'
      }
    }

    stage('Docker Push') {
      steps {
        sh 'docker push madhanmohanreddyeeda/github-repo-frontend:latest'
      }
    }

  }
}