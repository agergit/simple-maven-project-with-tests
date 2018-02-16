pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        bat 'c:\\plm\\maven\\bin\\mvn.cmd test'
      }
    }
    stage('install') {
      steps {
        bat 'c:\\plm\\maven\\bin\\mvn.cmd install'
      }
    }
  }
}