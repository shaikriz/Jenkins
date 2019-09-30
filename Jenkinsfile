pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        ws(dir: 'Jenkins_master') {
          sh '''ls -lrt
echo $PATH
java -version
env
mvn clean install'''
        }

      }
    }
  }
}