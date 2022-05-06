pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        echo 'build gradle..'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'

      }
    }    
  }
}
