pipeline {
    agent any
    stages {
        stage('Login') {
            steps {
                withCredentials([usernamePassword(credentialsId: '8fbd22aa-e646-4587-8f2b-3b578dbebe9e', passwordVariable: 'krishna', usernameVariable: 'root')]) {
                    // Use the credentials here, such as:
                    sh "echo Username: $USERNAME"
                    sh "echo Password: $PASSWORD"
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
