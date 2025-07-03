pipeline {
    agent any 
    environment {
        MOVIE="bahubali"
        SCM="github"
    }
    stages {
        stage ('build') {
            steps {
                echo "the movie ${MOVIE} is very nice film"
                echo "the scm tool in devops is ${SCM}" 
            }
        }
    }
}
