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
        deleteDir()
      }
    }
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}