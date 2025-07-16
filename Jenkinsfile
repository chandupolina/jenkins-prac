pipeline {
    agent any 
    stages {
        stage ('build') {
            steps {
                echo "building the code"
            }
        }
        stage ('parallel-stages') {
            parallel {
                stage ('A') {
                    steps {
                        echo " A stage is running"
                        sh 'sleep 10'
                    }
                }
                stage ('B') {
                    steps {
                        echo " B stage is running"
                        echo " b stage print"
                    }
                }
                stage ('C') {
                    steps {
                        echo " C stage is running"
                    }
                }
            }
        }
    }
}
