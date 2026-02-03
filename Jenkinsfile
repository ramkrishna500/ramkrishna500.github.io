pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/ramkrishna500/ramkrishna500.github.io.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                rm -rf /var/www/html/*
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
