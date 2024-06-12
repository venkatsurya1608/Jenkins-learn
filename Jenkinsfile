pipeline {
    agent {
        label 'AGENT-1'
    } 
    stages {
        stage('Build') { 
            steps {
                sh 'echo this venkat-build' 
            }
        }
        stage('Test') { 
            steps {
                sh 'echo this venkat-test' 
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo this is production'
            }
        }
    }
}

