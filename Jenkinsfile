pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo "Hello World stage"
                sh 'hostname'
            }
        }
        stage('Test') {
            steps {
                echo "Hello test stage"
                sh 'pwd'
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
