pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo "**** Coming from build stage****"
            }
        }
        stage('groovy-test') {
            steps {
                script{
                    def course = "k8s"
                    if (course == "k8s")
                        println("Thanks for enrolling")
                    else
                        println("Do enroll for k8s")
                }
            }
        }
    }
}
