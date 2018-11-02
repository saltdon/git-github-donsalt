pipeline {
  agent any
  stages {
    stage('compile stage') {
      steps {
        withMaven(maven : 'maven:3.1.2') {
            sh 'mvn clean compile'
        }
      }
    }
    stage('test in stage') {
      steps { 
        withMaven(maven : 'maven:3.1.2') {
           sh 'mvn test'
          
         
     stage('deployment stage') {
      steps { 
        withMaven(maven : 'maven:3.1.2') {
           sh 'mvn deployment'
      }
    }
  }
}
