pipeline {
    agent {
        label 'java-slave'
    }
    environment {
        GITHUB_CREDS = credentials('github_creds')
        SONAR_CREDS = credentials('sonar-scan-token')
    }
    stages {
        stage ('build') {
            steps {
                echo "my github credentials are ${GITHUB_CREDS}"
                echo "my github username is ${GITHUB_CREDS_USR}"
                echo "my github password is ${GITHUB_CREDS_PSW}"
                echo "my soanr credential are ${SONAR_CREDS}"
            }
        }
    }

}
