pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo 'Pipeline for Test Env'
        build 'codebuild-sam'
        echo 'Finished build'
      }
    }

  }
}