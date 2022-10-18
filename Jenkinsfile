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
                sh "cp /home/slave4/workspace/tomtest1/target/hello-world-war-1.0.0.war /opt/tomcat/webapps"
            }
        }
        stage ('test') {
            steps {
                echo "done"
            }
        }
    }
}
