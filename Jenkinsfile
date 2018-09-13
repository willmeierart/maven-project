pipeline {
  agenty any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
      post {
        success {
          echo 'Now Archiving...'
          archiveArtifacts artifcats: '**/target/*.war'
        }
      }
    }
  }
}