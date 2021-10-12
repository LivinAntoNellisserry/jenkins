pipeline {
    agent any
    environment{
        PATH = "C:/Program Files/apache-maven-3.8.3/bin:$PATH"
    }

    stages {
        stage('Build') {
            steps {
                sh "mvn clean install"
            }
        }
    }
}
