pipeline {
    agent any 
    tools {
        maven 'Maven 3.3.9'
    }
    stages {
        stage('Checkout') { 
            steps {
                git branch: 'main',
                credentialsId: '38ffa708-7e33-4cb0-ab94-f53110f6f5ea',
                url: 'https://github.com/Hkudumu/Sprinboot.git'
            }
        }
         stage('Build') { 
            steps {
               withMaven {
                  sh "mvn install"
                }    
            }
        }
       
    }
}
