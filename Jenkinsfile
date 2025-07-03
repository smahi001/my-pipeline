pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "**** Displaying the ip where this stage is executing ****"
                sh "hostname -i"
            }
        }
    }
}
