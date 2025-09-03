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
    stages {
        stage('Build') {
            steps {
                echo 'Build'
            }
        }
        stage('Test') {
            steps {
                echo 'Build'
            }
        }
        stage('Integration Test') {
            steps {
                echo 'Integration'
            }
        }
    } post {
        always {
            echo 'I am awesome. I run always'
        }
        success {
            echo 'I run when you are successful'
        }
        failure {
            echo 'I run when you fail'
        }
    }
}
