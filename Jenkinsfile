pipeline 
{
    agent any
    environment
    {
        MAVEN_HOME = /opt/apache-maven-3.9.8
       PATH = $PATH:/opt/apache-maven-3.9.8/bin
    }
    
    stages 
    {
        stage('1') 
        {
            steps 
            {  
                sh 'echo $MAVEN_HOME'
            }
        }
        stage('2') 
        {
            steps
            {
                sh 'echo $PATH
            }
        }
    }
}
