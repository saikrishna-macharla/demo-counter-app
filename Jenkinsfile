pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                    
                    git branch: 'main', url: 'https://github.com/saikrishna-macharla/demo-counter-app.git'
            }
        }
        stage('UNIT testing'){
            
            steps{
                    
                    sh 'mvn test'
                }
            }
       }
}
