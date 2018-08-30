pipeline {
    agent any
    environment {
    venv = 'source venv/bin/activate'
    }
    stages {
        stage('virtual env') {
            steps {
	        sh 'ls'
		sh 'test ! -d venv || rm -rf venv'
		sh '/var/lib/jenkins/.local/bin/virtualenv venv'
		sh 'ls'
              
            }
        }
        stage('test') {
            steps {
                sh 'cd venv'
		sh 'opsspace-test'         
            }

        }
     }
}

