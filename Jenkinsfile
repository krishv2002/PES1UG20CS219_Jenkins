pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -f Makefile -f makefile1'
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
