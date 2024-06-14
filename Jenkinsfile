pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        timeout(time: 1, unit: 'SECONDS')
        disableConcurrentBuilds()
    }
    // environment { 
    //     Deploy_To = 'dev'
    // }    
    stages {
        stage('plan') { 
            steps {
                """
                ls -la
                """
            }
        }
        stage('apply') { 
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

    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'I will run when pipeline is success'
        }
        failure { 
            echo 'I will run when pipeline is failure'
        }
    }
}

