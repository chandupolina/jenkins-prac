pipeline {
    agent any
    stages {
        stage ('Build') {
            steps  {
                retry(3) {
                    echo "using retry block under steps block"
                    error "using error to make the build failure"

                }
                echo  " i will come after 3 retrys "
            }
        }
    }
}
