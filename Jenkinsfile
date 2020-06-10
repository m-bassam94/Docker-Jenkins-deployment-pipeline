pipeline{
    agent any
    stages{
        stage("test"){
            steps{
                sh "cd tests && python3 test.py"
            }
        }
        stage("deploy"){
            steps{
                sh "sudo docker-compose up"
            }
        }

    }

}
