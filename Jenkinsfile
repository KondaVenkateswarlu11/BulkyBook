pipeline{
    agent none
    stages{
        stage("build stage"){
            agent{
                node{
                    label 'jenkins'
                    customWorkspace /home/
                }
            }
            steps{
                echo "This is stage is running in jenkins master node"
                sh 'hostname -i'
                echo "Git cloning is started"
                git 'https://github.com/KondaVenkateswarlu11/BulkyBook.git'
                echo "clone completed"
            }
        }
    }
}
