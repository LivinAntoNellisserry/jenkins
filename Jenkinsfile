pipeline 
{
    agent any
    tools 
    {
        maven 'maven-3.8.3'
        jdk 'jdk-11'
    }
    stages 
    {
        stage ('Initialize') 
        {
            steps
            {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }

        stage ('Build') 
        {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
            }
            
        }
    }
}
