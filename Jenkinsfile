pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo 'test1'
        catchError(buildResult: 'SUCCESS', message: 'shippai', stageResult: 'FAILURE') {
          echo 'test'
          sh 'exit 1'
        }

      }
    }

    stage('Test2') {
      steps {
        echo 'test2'
      }
    }

  }
}