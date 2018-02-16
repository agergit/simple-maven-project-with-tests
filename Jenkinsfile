pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        bat 'c:\\plm\\maven\\bin\\mvn.cmd test'
        cleanWs(cleanWhenAborted: true, cleanWhenFailure: true, cleanWhenNotBuilt: true, cleanWhenUnstable: true, cleanupMatrixParent: true, deleteDirs: true)
      }
    }
    stage('install') {
      steps {
        bat 'c:\\plm\\maven\\bin\\mvn.cmd clean install'
      }
    }
  }
}