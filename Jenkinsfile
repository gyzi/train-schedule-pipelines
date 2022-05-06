pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        echo 'build gradle..'
        sh './gradlew build --no-daemon'
        archiveArtifacts artfacts: 'dist/trainSchedule.zip'
      }
    }    
  }
}
