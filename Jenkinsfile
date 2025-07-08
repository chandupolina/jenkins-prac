pipeline {
    agent any
    environment {
        scans = 'execute'
    }
    stages {
        stage ('scans') {
            when {
                environment name: 'scan', value: 'execute'
            }
            steps {
                echo "executing the scans stage"
            }
        }
    }
}
