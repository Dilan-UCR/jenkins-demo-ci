pipeline {
    agent {
        docker {
            image 'node:18'
            args '-u root'
        }
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }
    }
}
