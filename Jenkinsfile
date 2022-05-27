pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'build application'
            }
        }
        stage('test'){
            steps {
                echo 'test'
            }
        }
        stage('Deploy'){
            steps {
                echo '$deploy'
            }
        }
        
    }        
        post {
            
            always {
                emailext body: '', subject: 'Pipeline status', to: 'jenkinsfirst9@gmail.com'
            }
        }
    
}
