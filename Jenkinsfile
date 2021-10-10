pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifact artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
