pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        bat 'make'
        archiveArtifacts(artifacts: '**/target/.o', fingerprint: true)
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