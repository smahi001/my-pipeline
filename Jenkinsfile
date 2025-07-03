pipeline{
    agent any
    stages {
        stage('build') {
            steps {
                retry(4) {
                    echo "welcome to jenkins pipelines"
                    error "This will give some error"
                    }
                echo "***printing after multiple retries***"
                }
            }
        }
    } 
