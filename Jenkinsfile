// pipeline {
//     agent any
//     stages {
//         stage('Build') {
//             steps {
// //                 sh 'make -f main/makefile2'
//                 sh 'make -C main'
//                 echo 'Build Stage Successful'
//             }
//         }
//         stage('Test') {
//             steps {
//                 sh '/var/jenkins_home/workspace/PES1UG20CS219-1/main/hello_exec'
// //                 sh '/var/jenkins_home/workspace/PES1UG20CS219-1/main/new_file'
//                 echo 'Test Stage Successful'
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 echo 'Deployed Sucessfully'
//             }
//         }
//     }
//     post {
//         failure {
//             echo 'Pipeline failed'
//         }
//     }
// }



pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'make -C main'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                sh '/var/jenkins_home/workspace/pes1ug20cs219-1/main/working_exec'
                sh '/var/jenkins_home/workspace/pes1ug20cs219-1/main/hello_exec'
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
