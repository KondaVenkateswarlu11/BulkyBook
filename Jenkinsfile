pipeline{
    agent any
    stages{
        stage("Example of retry and timeout stage"){
            steps{
               
                    retry(4){
                        try {
                            echo "retry block started again:"

                            timeout(time: 5, unit: 'SECONDS'){
                                echo "printing the timeout block"

                                sleep 60
                            }
                        } catch (FlowInterruptedException e) {
                            // handle the timeout error
                            error 'Timeout!'
                        }
                    }
                }
            }
        }
}
