pipeline {
    agent {
        label 'java-slave'
    }
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('build') {
            when {
                not {
                    equals expected:'prod' , actual : "${DEPLOY_TO}"
                }
            }
            steps {
                echo "Deploying to production"
            }
        }
    }
}
