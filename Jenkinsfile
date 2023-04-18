pipeline {
    agent any
    environment {
        DIRECTORY_PATH = ""
        TESTING_ENVIRONMENT = "Testing Environment"
        PRODUCTION_ENVIRONMENT = "pratikpawar"
    }
    stages {

        stage("Build") {
            steps {
                echo "fetch the source code from the directory path specified by the environment variable"
            }
            steps {
                echo "compile the code and generate any necessary artifacts"
            }
        }
        stage("Test") {
            steps {
                echo "Running unit tests for the application..."
            }
            steps {
                echo "Running integration tests for the application..."
            }
        }
        stage("Code Quality Check") {
            steps {
                echo "check the quality of the code for the application..."
            }
        }
        stage("Deploy") {
            steps {
                echo "deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage("Approval") {
            steps {
                echo "Approval stage..."
                sleep(time: 10, unit: 'SECONDS')
            }
        }
        stage("Deploy to Production") {
            steps {
                echo "Deploying to Production environment ${PRODUCTION_ENVIRONMENT}"
            }
        }
        

    }
}