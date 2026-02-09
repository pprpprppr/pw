pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                // This fetches the code from the Git repo defined in Step 4
                checkout scm
            }
        }
        stage('Run Python Script') {
            steps {
                echo 'Running your python script now...'
                // Executes the script using the system's python3
                sh 'python3 hello.py'
            }
        }
    }
    post {
        success {
            echo 'Build completed successfully!'
        }
    }
}
