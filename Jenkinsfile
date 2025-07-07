pipeline {
    agent {
        label 'java-slave'
    }
    environment {
        DOCKER_CREDS=credentials('docker_creds')
        DOCKER_REPO='cpolina/apach'
    }
    stages {
        stage ('DockerBP') {
            steps {
                sh "docker pull nginx"
                echo "----------------------printing images before changing the tag ---------------"
                sh "docker images"
                sh "docker tag nginx cpolina/apach:b7"
                echo "------------------printing images after changing the tag-------------------"
                sh "docker images"
                echo"---------------------Dcoker login----------------------------------"
                sh "docker login -u ${DOCKER_CREDS_USR}" -p ${DOCKER-CREDS-PSW}
                echo "----------------------pushing image to REPO---------------------"
                sh "docker push ${DOCKER_REPO}:b7"
            }
        }
    }
}
