pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                git credentialsId: 'github', url: 'https://github.com/sskumardgl/simple-app.git'
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'python3 test_app.py'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
