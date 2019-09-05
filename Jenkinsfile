pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        failOnError: false,
        continueOnError: true,
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
