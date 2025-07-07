pipeline {
    agent any
    environment {
        BRANCH_NAME = 'main'
    }
    stages {
        stage('Deploy') {
            when {
                not {
                    branch 'develop'
                }
            }
            steps {
                echo "This stage runs if NOT on 'develop' branch. Current branch: ${BRANCH_NAME}"
            }
        }
    }
}
