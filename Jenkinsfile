pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "Hello World"'
                 sh '''
                     echo "Multiline shell steps works too"
                     sudo apt install awscli
                     aws configure set region $AWS_DEFAULT_REGION
                     aws configure set aws_access_key_id $AWS_ACCESS_KEY_ID
                     aws configure set aws_secret_access_key $AWS_SECRET_ACCESS_KEY
                 '''
             }
         }      
     }
}
