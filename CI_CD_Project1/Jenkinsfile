pipeline{
    agent any

    stages{

        stage("Clone Repo")
        {
            steps{
                git branch: 'main', url: 'https://github.com/kevalp566/jenkins-ci-demo.git'
            }
        }

        stage("Install")
        {
            steps{
                sh 'npm install'
            }
        }

        stage("Test")
        {
            steps{
                sh 'npm test'
            }
        }

        stage("Deploy")
        {
            steps{
                echo 'Deploy step: You can add scp/docker/aws commands here'
            }
        }

    }
}
