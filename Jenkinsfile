pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o output PES1UG22CS0-pp'  // Compile C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './oput'  // Run the compiled program
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
