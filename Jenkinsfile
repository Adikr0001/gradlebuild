pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch:'main',url:'https://github.com/Adikr0001/gradlebuild.git'
            }
        }

        stage('Build') {
            steps {
                sh 'gradle build'
            }
        }

        stage('Test') {
            steps {
                sh 'gradle test'
            }
        }

        stage('Run Application') {
            steps {
                sh 'gradle run'
            }
        }

        stage('Custom Message') {
            steps {
                echo 'Gradle Jenkins Pipeline Executed Successfully!'
            }
        }

    }
}
