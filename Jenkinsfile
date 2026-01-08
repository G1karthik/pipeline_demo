pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git branch: 'main',
                    url: 'https://github.com/G1karthik/pipeline_demo.git'
            }
        }
        
        stage('verify workspace'){
            steps{
                sh '''
                echo "Present user"
                whoami
                
                echo "present working directory"
                pwd

                echo "Listing the files...."
                ls -ltr

                echo "Reading the app.txt file"
                cat app.txt
                '''
                }
        }
    }
}
