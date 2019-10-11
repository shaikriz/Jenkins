pipeline {
  agent none
  stages {
    stage('Build') {
      steps {
        sh '''pwd
/home/dc-user/apache-maven-3.2.1/bin/mvn clean install
ls -lrt
echo $PATH
java -version
env'''
      }
    }
  }
}