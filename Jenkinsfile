pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', url: 'https://github.com/ak12021996/demo-counter-app.git'
                }
            }
        }

        stage('unit testing'){

            steps{

                script{
                    sh 'mvn test'
                }

            }
        }
    }
}
 
