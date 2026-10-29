pipeline {
    agent {
        label 'ubuntu-agent'
    }

    stages {
        stage('Agent Verification') {
            steps {
                sh 'hostname'
                sh 'java -version'
                echo 'Pipeline executed on Jenkins agent'
            }
        }

        stage('Hello World') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
