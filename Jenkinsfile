pipeline {
    agent {
        label 'java-slave'
    }
    environment {
        DEPLOY_TO ='production'
    }
    stages {
        stage ('deployment') {
            when {
                expression { 
                    BRANCH_NAME ==~ (production | staging)
                }
            }
            steps {
                echo  " Deploying to production"
            }
        }        
    }
}
