Jenkinsfile (Declarative Pipeline)

pipeline {
    agent { docker { image 'python:3.5.1' } }
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

