pipeline {
        agent any
                 stages {
                         stages('one') {
                                  steps {
                                           echo 'Heello, this is from francis okole'
                                  }
                         }
                         stage('two') {
                                 steps {
                                         imput('Do you want to proceed?')
                                 }
                         }
                         stage('Three') {
                                when (
                                       not {
                                             branch "master"
                                       
                                      }
                                }      
                                steps { 
                                       echo "Hello how are you"
                                }
                         }
