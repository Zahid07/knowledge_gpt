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
                    //run the command to build the docker image
                    // sh 'docker build -t knowledge_gpt .'
                    //print in knowledge_gpt directory
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
