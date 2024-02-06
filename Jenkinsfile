pipeline {
    agent any 
    stages {
        stage('Run Python Script') {
            steps {
                sh 'python3 step1.py' 
            }
        }
        stage('Touch M2 Environment') {
            steps {
                sh '${SSH_URL}'
                touch 'var/test.txt'
            }
        }

    }
}
