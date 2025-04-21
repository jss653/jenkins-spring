pipeline {
  agent any
  tools {maven'M#'}
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'mvn package'
      }
    }
  }
}
