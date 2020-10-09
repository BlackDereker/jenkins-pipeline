pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        bat(script: 'make', returnStatus: true)
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