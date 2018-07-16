pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      environment {
        VERSION = 'readMavenPom().getVersion()'
      }
      steps {
        bat 'mvn clean install'
      }
    }
  }
  environment {
    VERSION = 'readMavenPom().getVersion()'
  }
}