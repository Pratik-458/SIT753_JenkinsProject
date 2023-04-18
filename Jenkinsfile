pipeline {
    agent any
    environment {
        DIRECTORY_PATH = ""
        TESTING_ENVIRONMENT = "Testing Environment"
        PRODUCTION_ENVIRONMENT = "pratikpawar"
    }
    stages {

        stage("Build") {
            step {
                echo "fetch the source code from the directory path specified by the environment variable"
            }
            step {
                echo "compile the code and generate any necessary artifacts"
            }
        }
        stage("Test") {
            step {
                echo "Running unit tests for the application..."
            }
            step {
                echo "Running integration tests for the application..."
            }
        }
        stage("Code Quality Check") {
            step {
                echo "check the quality of the code for the application..."
            }
        }
        stage("Deploy") {
            step {
                echo "deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage("Approval") {
            step {
                echo "Approval stage..."
                sleep(time: 10, unit: 'SECONDS')
            }
        }
        stage("Deploy to Production") {
            step {
                echo "Deploying to Production environment ${PRODUCTION_ENVIRONMENT}"
            }
        }
        

    }
}