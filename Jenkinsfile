pipeline {
    agent any
    stages {
        stage ('Build') {
            options {
                retry(3) 
            }
            steps {
                echo "Before setting currrent build to failure"
                script {
                    currrentBuild.result ='FAILURE'
                }
                echo " After setting current build as failure"
            }
        }
    }
}
