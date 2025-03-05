pipeline {
    agent any
    environment {
        
        MAVEN_HOME = '/opt/apache-maven-3.9.8'

        // Update the PATH to include Maven's bin directory
        PATH = "${env.PATH}:${MAVEN_HOME}/bin"
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
