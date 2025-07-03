pipeline {
    agent any
    parameters {
        string(name :'BRANCH_NAME ', defaultValue: 'main', description: 'Git branch to build')
        booleanParam(name: 'RUN_TESTS', defaultValue: true, description: ' Run tests after build')
        choice(name: 'ENV', choices:['dev','qa', 'prod'], description: 'Select Environment')
        password(name: 'SECRET_KEY', defaultValue: '', description: 'Enter secret key')
        text(name:'NOTES', defaultValue:' ', description: 'optional deployment notes')
    }
    stages {
        stage ('Build') {
            steps {
                echo "Branch: ${params.BRANCH_NAME}"
                echo  "Run tests: ${params.ENV}"
                echo  "Secret key (hidden)"
                echo "Notes: ${params.NOTES}"
            }
        }
    }

}
