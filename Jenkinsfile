pipeline {
    agent {
        docker { 
            image 'php:7.3.4-fpm'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'ls -la /'
                sh 'ls -la /var/www'
                sh 'ls -la'
                sh 'php test.php'
                sh 'php -i'
            }
        }
    }
}
