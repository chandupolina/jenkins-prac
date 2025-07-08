pipeline {
    agent any 
    environment {
        DEPLOY_TO = 'xyz'
    }
    stages {
        stage ('deploytodev') {
            steps {
                echo "deploying to dev "
            }
        }
        stage ('deploytoprod') {
            when {
                anyOf {
                    branch 'production'
                    // if any one condition met it will execute the stage 
                    environment name:'DEPLOY_TO' , value: 'production'
                }
            }
            steps {
                echo "Deploy to prod env"
            }
        }
    }
}
