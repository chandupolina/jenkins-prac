pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build') {
            steps {
                echo "building pipeline"
            }
        }
        stage ('scan') {
            steps {
                echo "scan the pipeline"
            }
        }
        stage ('dockerbuild') {
            steps {
                echo " docker pipeline"
            }
        }
        stage ('devdeploy') {
            steps {
                echo "deploying to dev"
            }
        }
    }

}
