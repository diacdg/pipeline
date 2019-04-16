pipeline {
    agent {
        docker { 
            image 'php:7.3.4-fpm'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'mkdir test 2>/dev/null'
                sh 'ls -la /'
                sh 'ls -la /var/www'
                sh 'ls -la'
                sh 'php test.php'
                sh 'php -i'
            }
        }
    }
}
