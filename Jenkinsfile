pipeline{
    agent any
    stages{
        stage("Starting Stage"){
            steps{
                echo "Started the pipeline"
            }
        }
        stage("retry stage"){
            steps{
                retry(3){
                    echo "Welocme to Pipeline"
                    error "Testing the Retry block"
                }
                echo "Printing after 3 retries..................."
            }
        }

    }
}
