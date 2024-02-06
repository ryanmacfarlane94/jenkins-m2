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
                sh 'magento-cloud ssh -e staging;touch var/test.txt;' 
            }
        }

    }
}
