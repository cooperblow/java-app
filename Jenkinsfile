pipeline {
  agent any
  stages {
    stage('Nonsense') {
      steps {
        echo 'Hello, World!'
      }
    }
    stage('Maven Build') {
      steps {
        sh 'mvn clean package -DskipTest'
      }
    }
    stage('Maven Deploy') {
      steps {
        sh 'mvn tomcat7:deploy'
      }
    }
  }
}