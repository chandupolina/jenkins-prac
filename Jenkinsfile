pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('DeploytoDev') {
            steps {
                echo " Deploying to Dev"
            }
        }
        stage ('ProdDeploy') {
            when {
                allOff {
                    //if there are 10 conditions all 10 conditions should be satisfied
                    branch = 'production'
                    environment name : 'DEPLOY_TO', value : 'production'
                }
            }
            steps {
                echo "Deploying to production"
            }
        }
    }
}
