pipeline {
  agent {
    node {
      label 'Make'
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        sh 'make'
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