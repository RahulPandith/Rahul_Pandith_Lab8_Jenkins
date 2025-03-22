pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo 'Building the project for PES1UG22CS462...'
                sh 'g++ -o output program.cpp' // Compile your C++ file
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests for PES1UG22CS462...'
                sh './output' // Execute compiled file
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project for PES1UG22CS462...'
                sh 'echo "Deployment successful for PES1UG22CS462!"' // Simulated deployment
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed for PES1UG22CS462!'
        }
    }
}
