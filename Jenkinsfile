pipeline {
    agent any
    environment {
        name='chandu'
        course='devops'
    }
    stages {
        stage ('BUild') {
            environment {
                course = 'gcp'
                name='pavan'
            }
            steps {
                echo "hello ${name}"
                echo "i am doing ${course}"
                sh 'printenv'
            }
        }
    }
}
