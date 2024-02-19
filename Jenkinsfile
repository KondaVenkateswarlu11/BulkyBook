pipeline{
    agent none
    stages{
        stage("build stage"){
            agent{
                node{
                    label 'jenkins'
                }
            steps{
                echo "This is stage is running in jenkins master node"
                sh 'hostname -i'
                git 'https://github.com/KondaVenkateswarlu11/BulkyBook.git'
            }
            }
        }
    }
}
