pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'print some text'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts 'dist/trainSchedule.zip'
      }
    }
  }
}
