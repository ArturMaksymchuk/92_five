pipeline {
    agent any
    environment {
      PROJECT_NAME = "92_five"
      
    }

    stages {
        stage('1-Build') {
            steps {
                
                echo "Start of Stage Build..."
                git credentialsId: 'sl1', url: 'https://github.com/ArturMaksymchuk/92_five.git'
                sh "ls -la"
                sh "pwd"
                sh "composer install"
                echo "Building......."
                echo "End of Stage Build..."
            }
        }
        stage('2-Test') {
            steps {
                echo "Start of Stage Test..."
                echo "Testing......."
                echo "Privet ${PROJECT_NAME}"
                echo "Owner is ${OWNER_NAME}"
                echo "End of Stage Build..."
            }
        }
        stage('3-Deploy') {
            steps {
                echo "Start of Stage Deploy..."
                echo "Deploying......."
                sh "ip a"
                sh '''
                   echo "Line1"
                   echo "Line2"
                '''
                echo "End of Stage Build..."
            }
        }
        stage('4-Celebrate') {
            steps {
                echo "CONGRATULYACIYA!"
            }
        }	
    }
}
