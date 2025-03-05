pipeline {
    agent any
    environment {
        
        MAVEN_HOME = 'hello'
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
