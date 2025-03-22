pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo 'Building the project for PES1UG22CS462...'
                sh 'ls -R'  // Debug: Show all files inside Jenkins workspace
                sh 'g++ -o output CC_TA/main/hello.cpp'  // Corrected path
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests for PES1UG22CS462...'
                sh './output' // Run compiled file
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project for PES1UG22CS462...'
                sh 'echo "Deployment successful for PES1UG22CS462!"'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed for PES1UG22CS462!'
        }
    }
}
