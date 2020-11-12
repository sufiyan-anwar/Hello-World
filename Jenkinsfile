pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat "mvn clean package"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test"
            }
        }
        stage('Release') {
            steps {
                bat "xcopy /E "C:\Users\sufiyan.anwar\Desktop\Java Test" "C:\Users\sufiyan.anwar\Desktop\Deployed Server\""
            }
        }
    }
}
