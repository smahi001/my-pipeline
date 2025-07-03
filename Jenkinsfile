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
        stage('development') {
            agent {
                label 'ssh-slave'
            }
            steps {
                echo "I am writing Jenkins pipelines using master and slave"
                sh "hostname -i"
            }
        }
    }
}
