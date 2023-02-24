pipeline {
    agent any

    environment {
        PATH = "${PATH}:${HOME}/.local/bin"
    }

    stages {
        stage('Cloning the repo') {
            steps {
                git branch: 'Jenkinsworkflow', url: 'https://github.com/Zahid07/knowledge_gpt.git'
                bat 'pip3 install poetry'

            }
        }

        stage('Lint with flake8') {
            steps {
                bat 'pip3 install flake8'
                bat 'flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics'
            }
        }

        // stage('Format with black') {
        //     steps {
        //         sh 'pip3 install black'
        //         sh 'black .'
        //     }
        // }
    }
}