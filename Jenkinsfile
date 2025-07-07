pipeline {
    agent any
    environment {
        name = 'chandu'
        course = 'devops'
    }
    stages {
        stage ('build') {
            environment {
                cloud = 'gcp'
            }
            steps {
                echo "hello this is ${name} from ${course} course"
                echo "i chose ${cloud} cloud"
            }
        }
        stage ('second stage') {
            steps {
                echo "hello ${name}"
                echo "i am doing ${course} course"
                echo "i chose ${cloud} cloud"

            }
        }
    }
}
