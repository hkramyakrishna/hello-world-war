pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                sh "git clone https://github.com/hkramyakrishna/hello-world-war.git"
            }
        }
        stage('test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
