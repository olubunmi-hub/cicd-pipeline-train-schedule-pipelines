pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifact artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
