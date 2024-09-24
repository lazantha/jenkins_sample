pipeline {
    agent any  // This will run on any available agent

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                https://github.com/lazantha/jenkins_sample.git
            }
        }

        stage('Build') {
            steps {
                // Build your application (e.g., using Maven)
                echo 'buiding....'  // Adjust according to your build tool
            }
        }

        stage('Test') {
            steps {
                // Run your tests
                echo 'testing....'  // Adjust according to your testing tool
            }
        }

        stage('Deploy') {
            steps {
                // Deploy your application (e.g., using a script)
                echo 'deploying....'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
