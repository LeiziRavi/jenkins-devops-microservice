// Scripted Pipeline
//  Old way to write jenkinsfile
// node {
//         echo 'Build'
//         echo 'Test'
//         echo 'Integration Test'
// }

// Declarative pipeline

pipeline {
    // agent any
    agent {
        docker {
            image 'maven:3.6.3'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                echo 'build'
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
