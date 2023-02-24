//create a simple jenkinsfile with ubuntu 20.04 as a node and install python 3.11 and poetry
pipeline {
    agent {
        docker {
            image 'ubuntu:20.04'
            args '-u root'
        }
    }
    stages {
        stage('Build') {
            steps {
                //in build stage, clone the repo Jenkinsworkflow branch from
                git branch: 'Jenkinsworkflow', url: 'https://github.com/Zahid07/knowledge_gpt.git'	
                //go to knowledge_gpt directory
                dir('knowledge_gpt') {
                    //install python 3.11
                    sh 'sudo add-apt-repository ppa:deadsnakes/ppa'
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
