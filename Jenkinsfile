pipeline {
    agent {
        label 'java-slave'
    }
    tools {
        maven 'maven-3.9.9'
    }
    stages {
        stage ("Maven") {
            steps {
                echo " Hello welcome to maven section"
                sh "mvn --version"

            }
        }
        stage ("cartmaven") {
            tools {
                jdk 'jdk-17'
            }
            steps {
                echo "hello welcome to cartmaven"
                sh "mvn --version"
            }
            
        }
    }
}
