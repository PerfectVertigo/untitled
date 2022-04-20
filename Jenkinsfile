pipeline {
  agent any
  stages {
    stage('Run Maven') {
      parallel {
        stage('Run Maven') {
          steps {
            sh 'mvn compile test package'
          }
        }

        stage('Maven Version') {
          steps {
            sh 'mvn --version'
          }
        }

      }
    }

  }
}