pipeline {
    agent any 
    stages {
        stage ('build') {
            steps {
                echo "build stage message"
            }
        }
        stage ('build2') {
            steps {
                sleep 10
                echo "run stage message"
            }
        }
    }
}
