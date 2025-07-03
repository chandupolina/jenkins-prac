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
                sh "java --version"

            }
        }
        stage ("cartmaven") {
            tools {
                jdk 'jdk-21'
                maven 'maven-3.6.3'
            }
            steps {
                echo "hello welcome to cartmaven"
                sh "java --version"
                sh "mvn --version"
            }
            
        }
    }
}
