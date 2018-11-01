pipeline {
  agent any
  parameters {
    file(name: 'ZIP')
  }
  stages {
    stage('Test file') {
      steps { 
        sh "echo ${params.ZIP}" 
      }
    }
  }
}
