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
echo $JAVA_HOME
echo $ANDROID_HOME
echo "================================================"
./gradlew check
echo "================================================"'''
        echo 'who'
      }
    }
  }
  environment {
    JAVA_HOME = '/opt/jdk1.8.0_144'
  }
}