pipeline 
{
    agent any
    tools {
        maven "MAVEN"
        jdk "JDK"
    }
    stages 
    {
        stage ('Initialize') 
        {
            steps
            {
                echo "Initialize"
                echo "PATH = ${M2_HOME}/bin:${PATH}"
                echo "M2_HOME = /Program Files/apache-maven-3.8.3"
            }
        }

        stage ('Build') 
        {
            steps {
                echo "Build"
                sh "mvn clean install"
            }
            
        }
    }
}
