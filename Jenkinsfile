pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        ws(dir: 'Jenkins_master') {
          sh '''pwd
mvn clean install
ls -lrt
echo $PATH
java -version
env
'''
        }

      }
    }
  }
}