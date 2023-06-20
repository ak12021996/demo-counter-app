pipeline{
    
    agent any 
    
    stages{
        
        stage('Git Checkout'){
            
            steps{  
                git branch: 'main', url: 'https://github.com/ak12021996/demo-counter-app.git'
                
            }
        }

        stage('unit testing'){

            steps{
                sh 'mvn test'
        
            }
        }

        stage('integration test'){
            steps{
                sh 'mvn verify -DiskpUnitTests'
            }
        }
            
    }
}
 
