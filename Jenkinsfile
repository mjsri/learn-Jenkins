pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying..'
            }
        }
    }
    // postbuild
    post {
        always {
            echo 'I will always say Hello again!'
        }
        failure {
            echo 'This runs when pipeline is failed, used generally to send some alerts'
        }
        success {
            echo 'I will say Hello when pipeline is success'
        }
    }
}