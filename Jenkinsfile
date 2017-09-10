pipeline {
    agent {
        docker { image 'golang:alpine' }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building Garson....'
                sh 'go get'
                sh 'go build'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Test Cases'
                sh 'go test .'
            }
        }
    }
}
