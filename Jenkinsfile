pipeline {
    agent any

    environment {
        GITHUB_ORG = 'timursamanchi'
        CONTAINER_REG = "ghcr.io/${GITHUB_ORG}/"

    }

    stages {
        stage ('Build Application') {
            steps {
                sh 'echo Performing Maven Build : ${GITHUB_ORG}'
            }
        }

        stage ('Build Container') {
            steps {
                sh 'echo Building Container Image : ${CONTAINER_REG}'
            }
        }

        stage ('Publishing Containe Image') {
            steps {
                sh 'echo Publishing COntainer Image : '
            }
        }
    }
}
