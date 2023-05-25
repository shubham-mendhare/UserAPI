pipeline{
  agent any
  stages{
    stage("build"){
      steps{
      echo 'Building the application...'
      }
    }
    stage("API Executions"){
      steps{
        newman run "Users_API.postman_collection.json" -d "UserCredentials.csv" -r htmlextra
      }
    }
  }
}

