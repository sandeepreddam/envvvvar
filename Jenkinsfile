pipeline {
    agent any
    environment {
        
        MAVEN_ SAN= ' MAVEN_HOME'
        PATH = 'PATH'
   }
    stages {
        stage('Clone Repository') {
            steps {  
                sh 'git clone https://github.com/RavitejaAdepudi/javawar'
            }
        }
        stage('Build with Maven') {
            steps {
                sh 'mvn -f /var/lib/jenkins/workspace/envvar/javawar/pom.xml install'
            }
        }
    }
}
