pipeline {
    agent { label 'slave4'}
    stages {
        stage('checkout') {
            steps {
                sh "pwd"
                sh "rm -rf hello-world-war"
                sh "git clone https://github.com/hkramyakrishna/hello-world-war.git"
            }
        }
        stage('build') {
            steps {
                sh "ls"
                sh "cd hello-world-war"
                sh "mvn clean package"
            }
        }
        stage('Deploy') {
            steps {
                sh "test envi"
            }
        }
        stage ('Deploy') {
            steps {
                echo "deploy"
            }
        }
    }
}
