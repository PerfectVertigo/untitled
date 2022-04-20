pipeline {
  agent any
  stages {
    stage('') {
      parallel {
        stage('Maven Verion') {
          steps {
            bat(script: 'mvn --version', returnStatus: true, returnStdout: true)
          }
        }

        stage('Run Maven') {
          steps {
            bat(script: 'mvn compile test package', returnStatus: true, returnStdout: true)
          }
        }

      }
    }

  }
}