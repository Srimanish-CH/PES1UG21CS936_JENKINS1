pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                build 'PES1UG21CS936-1345345'
                sh 'g++ main/hello.cpp -o output'
            }
        }

      
        stage('Deploy') {
            steps {
                echo 'deploy'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
