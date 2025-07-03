pipeline {
    agent any 
    stages {
        stage ('Build') {
            steps {
                echo "build stage "
            }
        }
        stage ('scan') {
            steps {
                echo 'scan the source code'
            }
        }
        stage ('dockerbuild') {
            steps {
                echo 'docoker pipeline'
            }
        }
        stage ('devdeploy') {
            steps {
                echo "deploying to dev"
            }
        }
        stage ('testdeploy') {
            steps {
                echo "deploying to test"
            }
        }
        stage ('DeployTOStage') {
            steps {
                echo "Deploying to Stage env"
            }
        }
        stage ('DeployToProd') {
            steps {
                echo "Deploying to Prod env"
            }
        }
    }
}
