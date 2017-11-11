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
./gradlew check --stacktrace
echo "================================================"'''
        echo 'who'
      }
    }
    stage('report') {
      steps {
        archiveArtifacts 'app/build/reports/*/*.html'
        fileExists 'app/build/reports/checkstyle/checkstyle32.html'
      }
    }
  }
}