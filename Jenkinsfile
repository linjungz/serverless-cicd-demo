pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Pipeline for Test Env'
        build 'codebuild-sam'
        echo 'Finished build'
      }
    }

    stage('Approval') {
      steps {
        waitUntil()
        input(message: 'Need Approval for Deployment', id: 'id', ok: 'ok')
      }
    }

  }
}