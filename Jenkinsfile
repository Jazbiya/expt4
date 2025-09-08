pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                  git branch: 'main', credentialsId: 'dcc79434-b63c-4869-a616-319cbccfd3e1', url: 'https://github.com/Jazbiya/expt4.git'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }
         stage('Run') {
            steps {
                bat 'java HelloWorld'
            }
        }
    }
}
