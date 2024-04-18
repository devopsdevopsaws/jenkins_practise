pipeline {
    agent { node { label 'AGENT' } }
    options {
        ansiColor('xterm')
    }
    stages {
        stage('Build') { 
            steps {
                echo 'building'
                sh 'ls -ltr'
                echo '\033[34mHello\033[0m \033[33mcolorful\033[0m \033[35mworld!\033[0m'
            }
        }
        stage('Test') { 
            steps {
                echo 'testing'
                sh 'pwd'
                echo '\033[34mHello\033[0m \033[33mcolorful\033[0m \033[35mworld!\033[0m'
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
                echo '\033[34mHello\033[0m \033[33mcolorful\033[0m \033[35mworld!\033[0m'
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