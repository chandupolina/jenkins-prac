pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "implementing timeout option"
                timeout (time:5 , unit :'SECONDS')
                {
                    echo " sleeping for 60 seconds"
                    sleep 60
                }
            }
        }
    }
}
