pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        ws(dir: 'Jenkins_master') {
          sh '''pwd
$MVN_HOME/bin/mvn clean install
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