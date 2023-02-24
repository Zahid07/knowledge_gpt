pipeline {
    agent any

    environment {
        PATH = "${PATH}:${HOME}/.local/bin"
    }

    stages {
        stage('Cloning the repo') {
            steps {
                git branch: 'Jenkinsworkflow', url: 'https://github.com/Zahid07/knowledge_gpt.git'
                //go to knowledge_gpt directory
                dir('knowledge_gpt') {
                    //install python 3.11
                    // sh 'sudo add-apt-repository ppa:deadsnakes/ppa'

                    //install the library pip install poetry
                    // sh 'pip install poetry'
                    echo 'Building..'
                    

                }

            }
        }

        // stage('Lint with flake8') {
        //     steps {
        //         sh 'pip3 install flake8'
        //         sh 'flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics'
        //     }
        // }

        // stage('Format with black') {
        //     steps {
        //         sh 'pip3 install black'
        //         sh 'black .'
        //     }
        // }
    }
}