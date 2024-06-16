pipeline {
    agent any 
    stages {
        stage('Checkout') { 
            steps {
                git branch: 'main',
                credentialsId: '38ffa708-7e33-4cb0-ab94-f53110f6f5ea',
                url: 'https://github.com/Hkudumu/Sprinboot.git'
            }
        }
         stage('MVN Clean') { 
            steps {
               mvn install
            }
        }
       
    }
}
