pipeline {
    agent { docker { image 'python:3.5.1' } }
    parameters { choice(name: 'CHOICES', choices: ['one', 'two', 'three'], description: '') }
    stages {
        stage('Stage 1 - Check Python version') {
            steps {
                sh 'python --version'
            }
        }
        stage('Stage 2 - Run hello world') {
            steps {
                sh 'python src/hello_world.py'
            }
        }
    }
}
