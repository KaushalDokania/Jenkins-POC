pipeline {
    agent { dockerfile true }
    stages {
        stage('Stage 1 - Check Python version') {
            steps {
                sh 'python --version'
            }
        }
        stage('Stage 2 - Check AWSCLI') {
            steps {
                sh 'aws --version'
            }
        }
        stage('Stage 3 - Run hello world') {
            steps {
                sh 'python src/hello_world.py'
            }
        }
    }
}
