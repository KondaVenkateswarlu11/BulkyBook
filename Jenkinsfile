pipeline{
    agent any
    stages{
        stage("Example of retry and timout stage"){
            steps{
                retry(4){
                    echo "retry block started again:"

                    timeout(time: 5, unit: 'SECONDS'){
                        echo "printing the timout block"

                        sleep 60
                    }
                    
                }
            }
        }
    }
}
