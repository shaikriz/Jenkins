pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        deleteDir()
        sh '''ls -lrt
echo $PATH
java -version
env
mvn clean install'''
        sleep 10
      }
    }
  }
}