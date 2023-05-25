pipeline {
    agent {label 'debian'}

    stages {
        stage('USER API Testing') {
            steps {
               newman run "Users_API.postman_collection.json" -d "UserCredentials.csv" -r htmlextra
            }
        }
    }
}
