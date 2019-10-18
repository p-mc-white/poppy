pipeline {
  agent any
  stages {
    stage('---clean---') {
      steps {
        sh "pwd"
        sh "ls"
        sh "mvn clean -f my-app"
      }
    }
    stage('--test--') {
      steps {
        sh "mvn test -f my-app"
      }
    }
    stage('--package--') {
      steps {
        sh "mvn package -f my-app"
      }
    }
  }
}
