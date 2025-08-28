pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
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
                echo "Hello deploy stage"
                sh 'date'
            }
        }
    }
}
