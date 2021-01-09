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

    stage('Deploy') {
      steps {
        input 'Need Approval for Deployment'
        echo 'Now deploy application'
      }
    }

  }
}