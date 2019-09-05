pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        continueOnError: false,
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
