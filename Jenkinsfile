pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/123AnkitSharma/helloc.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'gcc hello.c -o hello'
            }
        }
        stage('Run') {
            steps {
                sh './hello'
            }
        }
    }
}
