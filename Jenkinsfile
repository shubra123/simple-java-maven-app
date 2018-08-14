pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                pre {
                    always {
                    echo "Running Pre build steps"
                    }
                }
                echo "Building..."
            }
        }
        stage('DEV') {
            steps {
                echo "DEV Testing"
            }
            post {
                always {
                    echo "Running post DEV test: GIT taggging"
                }
            }
        }
         stage('SIT') {
            steps {
                echo "SIT Testing"
            }
            post {
                always {
                    echo "Running post SIT test: GIT taggging"
                }
            }
        }
        stage('UAT') {
            steps {
                echo "UAT Testing"
            }
            post {
                always {
                    echo "Running post UAT test: GIT taggging.. Done"
                }
            }
        }
    }
}
