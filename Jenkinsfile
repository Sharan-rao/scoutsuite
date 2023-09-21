pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "Hello World"'
                 sh '''
                     sudo apt-get update
                     echo "Multiline shell steps works too"
                 '''
             }
         }      
     }
}
