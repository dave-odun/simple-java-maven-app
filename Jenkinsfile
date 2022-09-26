pipeline {
  agent {
    docker {
      image 'node:current-alpine3.16'
    }

  }
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/dave-odun/simple-java-maven-app', branch: 'master')
        dockerNode(image: 'node:current-alpine3.16')
      }
    }

  }
}