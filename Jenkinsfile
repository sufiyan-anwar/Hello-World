pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat "mvn clean install"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test"
            }
        }
        stage('Release') {
            steps {
                bat 'xcopy /E "C:\\Users\\master\\AppData\\Local\\Jenkins\\.jenkins\\workspace\\Hello World WebHook" "C:\\Users\\master\\Desktop\\Deployed Server\\"'
            }
        }
    }
}
