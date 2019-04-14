pipeline {
    agent {
        docker { image 'php:7.3.4-fpm' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'php test.php'
            }
        }
    }
}
