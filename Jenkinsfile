pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/dave-odun/simple-java-maven-app', branch: 'master')
      }
    }

    stage('Docker Env') {
      steps {
        dockerNode(image: 'node:current-alpine3.16') {
          sh '''pwd 
ls'''
        }

      }
    }

  }
}