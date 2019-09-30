pipeline {
  agent any
  stages {
    stage('check environment') {
      steps {
        sh '''ls -lrt
echo $PATH
java -version
env'''
        sleep 10
      }
    }
  }
}