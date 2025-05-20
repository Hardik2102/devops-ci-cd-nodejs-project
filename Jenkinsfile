pipeline {
  agent any

  stages {
    stage('Clone Repo') {
      steps {
        git 'https://github.com/Hardik2102/devops-ci-cd-nodejs-project.git'
      }
    }

    stage('Build Docker Image') {
      steps {
        sh 'docker build -t hardik-node-app .'
      }
    }

    stage('Deploy Docker Container') {
      steps {
        sh 'docker stop hardik-node-app || true'
        sh 'docker rm hardik-node-app || true'
        sh 'docker run -d --name hardik-node-app -p 80:3000 hardik-node-app'
      }
    }
  }
}
