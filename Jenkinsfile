pipeline{
    agent any
    stages{
        stage("test"){
            steps{
                cd tests && python3 test.py
            }
        }

        stage("deploy"){
            steps{
                docker-compose up
            }
        }
    }

}