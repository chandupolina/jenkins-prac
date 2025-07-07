pipeline {
    agent any
    environment {
        name='chandu'
        course='devops'
    }
    stages {
        stage ('build') {
            environment {
                cloud='GCP'
            }
            steps {
                echo "name is ${name}"
                echo "and my course is ${course} using ${cloud} cloud"

            }
        }

    }
}
