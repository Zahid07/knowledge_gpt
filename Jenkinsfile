//create a simple jenkinsfile with build and test stages
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                //in build stage, clone the repo Jenkinsworkflow branch from https://github.com/Zahid07/knowledge_gpt.git
                git branch: 'Jenkinsworkflow', url: 'https://github.com/Zahid07/knowledge_gpt.git'
                //go to knowledge_gpt directory
                dir('knowledge_gpt') {
                    //run the command poetry install to install all the dependencies
                    // sh 'poetry install'
                    //install python3-pip
                    // sh 'sudo apt-get install python3-pip'
                    //check if python installed
                    sh 'python3 --version'

                    //install the library pip install poetry
                    // sh 'pip install poetry'
                    echo 'Building..'
                    

                }

            }

        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
    }
}
