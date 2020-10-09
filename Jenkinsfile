pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        archiveArtifacts(artifacts: '**/target/.o', fingerprint: true)
        bat 'make'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}