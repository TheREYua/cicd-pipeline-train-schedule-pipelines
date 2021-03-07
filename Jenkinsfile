pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Build started'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainShedule.zip'
      }
    }
  }
}
