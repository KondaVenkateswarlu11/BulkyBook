pipeline{
    agent {
        label 'jenkins'
    }
    tools{
        maven 'Maven 3.8.8'
    }
    environment{
        name = venkat
        course = devops
    }
    stages{
        stage("Build Stage"){
            environment{
                cloud = gcp
            }
            steps{
                echo "Welcome Mr.${name}"
                echo "Thanks for enrolling to the ${course} course"
                echo " certified in ${cloud}"
            }
        }
    }
}
