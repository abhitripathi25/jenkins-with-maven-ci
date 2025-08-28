pipeline {
    agent any

    tools {
        maven 'mvn-local'   // Name same hona chahiye jo Global Tool Config me diya tha
        jdk 'jdk-local'
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

