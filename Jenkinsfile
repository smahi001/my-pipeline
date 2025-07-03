pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "**** Displaying the ip where this stage is executing ****"
                sh "hostname -i"
            }
        }
        stage('test') {
            agent {
                label 'java-slave'
            }
            steps {
                echo "** Displaying the ip where this stage is running**"
                sh "hostname -i"
            }
        }
    }
}
