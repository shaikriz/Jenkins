pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          agent {
            label 'linux'
          }
          steps {
            sh '''pwd
mvn clean install
ls -lrt
echo $PATH
java -version
env'''
          }
        }
        stage('parallel test') {
          steps {
            sh 'echo "this is a parallel step"'
          }
        }
      }
    }
  }
}