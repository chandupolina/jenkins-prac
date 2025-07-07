pipeline {
    agent any 
    options {
        retry(3)
    }
    stages {
        stage ('Build') {
            steps {
                echo  "Before setting currrent build to failure"
                script {
                    currentBuild.result = 'FAILURE'
                }
                echo "After setting current build as failure"
            }
        }
    }
}
