pipeline {
    agent any 
    environment {
        DEPLOY_TO ='production'
    }
    stages {
        stage ('deploy') {
            when {
                environment name:'DEPLOY_TO', value:'production'
            }
            steps {
                echo "Deploy to production env"
            }
        }
    }
}
