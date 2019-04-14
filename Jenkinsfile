pipeline {
    agent {
        docker { 
            image 'php:7.3.4-fpm' 
            customWorkspace '/var/www/html'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh 'pwd'
                sh 'ls -la ../'
                sh 'ls -la'
                sh 'php test.php'
            }
        }
    }
}
