pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
                checkout scm
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
          stage('package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('deploy') {
            steps {
                echo "Running HelloWorld Java Program"
                sh 'java -cp target/classesHelloWorld'
            }
        }
    }
}
