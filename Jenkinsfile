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
            }
        }
    }
}