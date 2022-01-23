pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'print some text'
        sh './gradlew build --no- daemon'
        archiveArtifact artifacts 'dist/trainSchedule.zip'
      }
    }
  }
}
