pipeline{
    agent any
    stages{
        stage('demo'){
            steps{
                echo 'Hello'
            }
        }
        stage('Build'){
            steps{
                echo 'build app'
            }
        }
        stage('Deploy'){
            steps{
                echo 'deploy app'
            }
        }
        stage('Test'){
            steps{
                echo 'test app'
            }
        }
    }
    
    post{
        always{
            emailext body: 'Testing jenkins with mail', subject: 'Jenkins', to: 'gayu.sri340@gmail.com'
        }
    }
}
