pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build the stage!!'
      }
    }
    stage('Testing') {
      steps {
        sh 'Sleep 5'
        sh 'echo Tests Completed!'
      }
    }
    stage('Publish Event') {
      steps {
        script {
          publishEvent simpleEvent('testingCompleted')
        }

      }
    }
  }
}