pipeline {
    agent any   // run on any available Jenkins agent

    stages {
        stage('Build') {
            steps {
                echo '=== Build Stage ==='
                // simulate build (compile or package)
                bat 'echo Building the project...'
            }
        }

        stage('Test') {
            steps {
                echo '=== Test Stage ==='
                // run a simple Python test
                bat 'python3 hello.py'
            }
        }

        stage('Deploy') {
            steps {
                echo '=== Deploy Stage ==='
                // simulate deploy
                bat 'echo Deploying application...'
            }
        }
    }

    post {
        always {
            bat "Pipeline completed. Result: ${currentBuild.currentResult}"
        }
    }
}
