pipeline {
    agent any 
    stages {
        stage ('Build') {
            options {
                retry(3)
            }
            steps {
                echo "Before Setting Current Build to Failure"
                script {
                    currentBuild.result = 'FAILURE'
                }
                echo "After Setting Current Build to Failure"
            }
        }
    }
}
