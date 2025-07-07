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
                    equals expected: 'production' , actual : "${DEPLOY_TO}"
                }
            }
            steps {
                echo "Deploying to production"
            }
        }
    }
}
