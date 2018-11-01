pipeline {
  agent any
  }
  stages {
    stage('build') {
      steps {
        sh "./build-artifact.sh"
      }
    }
    stage('test in docker') {
      agent {
        docker {
          image 'ubuntu:16.04'
          reuseNode true
        }
      }
      steps {
        sh "./run-tests-in-docker.sh"
      }
    }
  }
}
