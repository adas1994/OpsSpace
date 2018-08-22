pipeline {
    agent { docker { image 'python:2.6.6' } }
    stages {
        stage('install') {
            steps {
                sh 'python setup.py install'
            }
        }
        stage('test') {
            steps {
                sh 'opsspace-test'         
            }

        }
     }
}

