pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        deleteDir()
        sh '''git clone https://github.com/shaikriz/Jenkins.git
cd Jenkins
ls -lrt
echo $PATH
java -version
env
mvn clean install'''
        sleep 10
      }
    }
  }
}