pipeline{
    agent any
    stages{
        stage("firstStage"){
            steps{
                echo "This is for script usage pipeline"
            }
        }
        stage("script stage"){
            steps{
                script{
                echo "here im writing the actual script code"
                def course = "k8s"
                if(course == "k8s"){
                    println ("Thanks for enrolling to ${course}")
                }
                else{
                    echo "Do enroll for the course ${course}"
                    sh 'sleep 5'
                }
                echo "pipeline successsfully completed.........."

            }

            }
        }
    }
}
