pipeline {
    agent any

    stages {
        stage('w/o docker') {
            steps {
                echo 'Without docker'
            }
        }
        stage('w/ docker') {
            agent {
                docker {
                    image 'node:18-alphine'
                }
            }
            steps {
                echo 'With docker'
            }
        }
    }
}
