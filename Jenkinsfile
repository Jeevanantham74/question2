pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code from repository...'
            }
        }
        stage('Install Dependencies') {
            steps {
                echo 'Installing required testing dependencies...'
                bat 'pip install pytest'
            }
        }
        stage('Run Unit Tests') {
            steps {
                echo 'Executing unit tests in verbose mode...'
                bat 'pytest -v'
            }
        }
    }
}
