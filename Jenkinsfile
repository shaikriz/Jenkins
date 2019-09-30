pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        deleteDir()
        sleep 10
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