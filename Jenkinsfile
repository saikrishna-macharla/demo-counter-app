pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                    
                    git branch: 'main', url: 'https://github.com/saikrishna-macharla/demo-counter-app.git'
                }
            }
        stage('UNIT TESTING'){
            
            steps{
                    
                    sh 'mvn test'
            }
        }    
        stage('Integration Testing'){
            
            steps{  
                    sh 'mvn verify -DskipUnitTests'
               }
           }  
     }
}   
