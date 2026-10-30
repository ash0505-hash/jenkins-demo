
pipeline {
    agent any

    stages {
        stage('Check Server') {
            steps {
                sh 'hostname'
                sh 'whoami'
                sh 'date'
                sh 'pwd'
            }
        }

        stage('Create File') {
            steps {
                sh 'mkdir -p devops'
                sh 'touch devops/hello.txt'
                sh 'ls -l devops'
            }
        }

        stage('Verify File') {
            steps {
                sh '''
                    if [ -f devops/hello.txt ]; then
                        echo "SUCCESS: File created!"
                    else
                        echo "ERROR: File not found"
                        exit 1
                    fi
                '''
            }
        }
    }
}
