pipeline {
    agent any

    environment {
        GITHUB_ORG = 'https://github.com/timursamanchi'
        CONTAINER_REGISTRY = "ghcr.io/${GITHUB_ORG}/"
        ARTIFACT_ID = readMavenPom().getArtifactId()
        JAR_NAME = "${ARTIFACT_ID}-${BUILD_NUMBER}"
        IMAGE_NAME = "${CONTAINER_REGISTRY}${ARTIFACT_ID}"
    }

    stages {
        stage ('Build Application') {
            steps {
                sh 'echo Performing Maven Build : ${ARTIFACT_ID}'
            }
        }

        stage ('Build Container') {
            steps {
                sh 'echo Building Container Image : ${IMAGE_NAME}'
            }
        }

        stage ('Publishing Containe Image') {
            steps {
                sh 'echo Publishing COntainer Image : ${CONTAINER_REGISTRY}'
            }
        }
    }
}