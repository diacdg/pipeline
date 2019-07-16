pipeline {
    agent any
    stages {
        stage('Test') {
            agent {
                docker { 
                    image 'php:7.3.4-fpm'
                }
            }
            steps {
                sh 'ls -la /var/www'
                sh 'ls -la'
                sh 'php test.php'
                sh 'php --version'
            }
        }
        stage('Local') {
            steps {
                sh 'ls -la /var/www' 
                sh 'ls -la'
                sh 'php --version'
            }
        }
    }
}
