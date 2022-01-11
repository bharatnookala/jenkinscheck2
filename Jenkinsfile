pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'message for compilation'
      }
    }

    stage('test') {
      steps {
        bat 'mvn -v'
      }
    }

  }
}