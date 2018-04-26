pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/narasimhavuppala/spring-rest.git', branch: 'master', changelog: true)
      }
    }
    stage('Build') {
      steps {
        bat 'mvn clean install'
      }
    }
  }
}