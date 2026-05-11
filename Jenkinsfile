pipeline {
    agent any

    tools {
        maven 'Maven3'
        jdk 'JDK21'
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Mallikarjun067/6thprogram.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
