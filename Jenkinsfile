pipeline
{
  agent any
environment {
        MAVEN_SAN 
    }
stages
  {
stage('1')
{
 {
sh ' git clone https://github.com/RavitejaAdepudi/javawar '
  }
}
stage('2')
{
 {
sh ' mvn -f /var/lib/jenkins/workspace/envvar/javawar/pom.xml install ' 
  }
}
}
}
