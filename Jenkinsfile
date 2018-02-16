pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        bat 'c:\\plm\\maven\\bin\\mvn.cmd test'
        sh 'which git.exe'
      }
    }
  }
}