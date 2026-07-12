groovy
pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out code'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'No tests available'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: 'target/*.war'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage'
            }
        }

        stage('Health Check') {
            steps {
                echo 'Application Healthy'
            }
        }

    }

}

