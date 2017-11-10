pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        echo 'clone it'
      }
    }
    stage('chek') {
      steps {
        sh './gradlew check'
      }
    }
  }
}