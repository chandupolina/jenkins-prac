pipeline {
    agent any
    environment {
        scans = 'execute'
    }
    stages {
        stage ('scans') {
            when {
                anyOf {
                    branch 'main'
                    environment name: 'scn', value: 'execute'
                }
            }
            steps {
                echo "executing the scans stage"
            }
        }
    }
}
