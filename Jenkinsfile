pipeline {
    agent any

    environment {
        // Define environment variables if needed
        MY_ENV_VAR = "some_value"
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Replace with actual build commands, e.g., for a Java project
                // sh 'mvn clean install'   // For example, using Maven
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Replace with your test command, e.g., for a Node.js project
                // sh 'npm test'            // For example, running tests with npm
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Replace with actual deployment command, e.g., to AWS, Kubernetes, etc.
                // sh './deploy.sh'         // Custom deploy script or commands
            }
        }
    }



    
    post {
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
        always {
            echo 'This will run regardless of the outcome.'
        }
    }
}
