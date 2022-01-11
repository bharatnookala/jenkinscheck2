pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'message for compilation'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            bat 'mvn -v'
          }
        }

        stage('functional test') {
          steps {
            bat 'java -version'
          }
        }

        stage('ipconfig') {
          steps {
            bat 'ipconfig'
          }
        }

      }
    }

  }
}