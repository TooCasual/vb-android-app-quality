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
        sh '''echo "================================================"
who
cat ~/.bashrc
echo "================================================"
./gradlew check
echo "================================================"'''
        echo 'who'
      }
    }
  }
}