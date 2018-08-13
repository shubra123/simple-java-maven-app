pipeline {
    agent any
    
    stages {
        stage('Build') { 
            steps {
                echo "Building..." 
            }
        }
        stage('Test') {
            steps {
                echo "Testing"
            }
            post {
                always {
                    echo "Running post test"
                }
            }
        }
         stage('Deliver') {
            steps {
                echo "Deliver stage"
            }
        }
    }
}
