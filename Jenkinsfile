pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/Prashantj8605/springbootdockerjenkins.git'
                sh './mvnw compile'
                echo 'MAven build successfully'
            }
        }
        stage('Test') {
            steps {
            	sh './mvnw test'
                echo 'Testcases executed Successful'
            }
        }
        stage('Package') {
            steps {
            sh './mvnw package'
                echo 'Application Deploy Successful'
            }
        }
        
    }
}
