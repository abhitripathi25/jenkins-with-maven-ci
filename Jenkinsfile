pipeline {
    agent any

    tools {
        maven 'Maven3'   // Name same hona chahiye jo Global Tool Config me diya tha
        jdk 'JDK17'
    }

    stages {
        stage('Compile') {
            steps {
                sh 'mvn compile'
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
        stage('Deploy') {
            steps {
                echo 'Hello World from Deploy'
            }
        }
    }
}

