// Scripted Pipeline
//  Old way to write jenkinsfile
// node {
//         echo 'Build'
//         echo 'Test'
//         echo 'Integration Test'
// }

// Declarative pipeline

pipeline {
    agent any
    // agent {
    //     docker {
    //         image 'maven:3.6.3'
    //     }
    // }
    // agent {
    //     docker {
    //         image 'node:13.8'
    //     }
    // }
    stages {
        stage('Build') {
            steps {
                // sh 'mvn --version'
                // sh 'node --version'
                echo 'build'
                echo '$PATH'
                echo 'BUILD_NUMBER - $env.BUILD_NUMBER'
                echo 'BUILD_ID - $env.BUILD_ID'
                echo 'BUILD_TAG - $env.BUILD_TAG'
                echo 'JOB_NAME - $env.JOB_NAME'
            }
        }
        stage('Test') {
            steps {
                echo 'test'
            }
        }
        stage('Integration Test') {
            steps {
                echo 'integration test'
            }
        }
    }
    post {
        always {
            echo 'I am awesome. I run always'
        }
        success {
            echo 'I run when you are successful'
        }
        failure {
            echo 'I run when you fail'
        }
    //changed{
    // echo 'I run when status changes'
    // }
    }
}
