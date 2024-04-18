pipeline {
    agent { node { label 'AGENT' } }
    stages {
        stage('Build') { 
            steps {
                echo 'building'
                sh 'ls -ltr'
            }
        }
        stage('Test') { 
            steps {
                echo 'testing'
                sh 'pwd'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploying'
                sh '''
                ls -ltr
                pwd
                hostname
                '''
                error 'error'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {
            echo 'I will run only on success'
        }
        failure {
            echo 'I will run only on failure'
        }
    }
}