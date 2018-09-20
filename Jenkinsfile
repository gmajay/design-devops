pipeline {
//	agent any    
    stages{
        
        stage('Git Checkout'){
            
            steps {
                git 'https://github.com/gmajay/design-devops.git'
            }
        }
        
        stage('Maven Build'){
            steps{
                sh 'mvn clean install'
            }
        }
        
        stage('Publish'){
            steps{
                archiveArtifacts 'target/springboot-petclinic-1.4.1.jar'
                junit 'target/surefire-reports/*.xml'
                
            }
        }
    }
}

