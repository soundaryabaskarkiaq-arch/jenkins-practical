pipeline {
    agent any

    stages {
        stage('Hello World') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Create Artifact') {
            steps {
                sh '''
                    mkdir -p output
                    echo "Jenkins practical assessment completed" > output/hello.txt
                    cat output/hello.txt
                '''
            }
        }
    }

    post {
        always {
            archiveArtifacts artifacts: 'output/**', allowEmptyArchive: false
        }
    }
}

