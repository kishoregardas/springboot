pipeline {
    agent any
    environment {
        PATH = "/opt/apache-maven-3.6.3/bin/:$PATH"
    }

    stages {
        stage('fetch code from github') {
            steps {
               git 'https://github.com/Namdev12/hello-world-war.git'
            }
        } 
        stage('build a package') {
            steps {
               sh 'mvn clean package'
            }
        }
        stage('tomcat deploy') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
