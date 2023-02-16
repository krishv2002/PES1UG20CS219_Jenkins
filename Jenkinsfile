pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
//                 sh 'make -f main/makefile2'
                sh 'make -C main'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                sh '/var/jenkins_home/workspace/PES1UG20CS219-1/main/hello_exec'
                sh '/var/jenkins_home/workspace/PES1UG20CS219-1/main/hello_exec1'
                echo 'Test Stage Successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployed Sucessfully'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
