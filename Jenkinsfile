pipeline {
    agent any

    stages {
        stage ('Build Application') {
            steps {
                sh 'echo Performing Maven Build'
            }
        }

        stage ('Build Container') {
            steps {
                sh 'echo Building Container Image'
            }
        }

        stage ('Publishing Containe Image') {
            steps {
                sh 'echo Publishing COntainer Image'
            }
        }
    }
}