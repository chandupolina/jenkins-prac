pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                echo "Hello world"
                sh "hostname -i"
            }
        }
        stage ('script stage') {
            steps {
                script {
                    def course = "maven"
                    if (course=="maven") {
                        println("thanks for enrolling in ${course}")
                    }
                    else {
                        println("try to learn ${course}")
                        sleep 10
                    }
                    
                    echo "script block has been executed"
                }
            }
        }
    }
}
