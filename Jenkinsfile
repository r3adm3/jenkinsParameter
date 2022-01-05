pipeline {
  agent any
  stages {
    stage('First Stage') {
      environment {
        testParameter1 = 'doodad'
      }
      steps {
        sh 'echo $HOME'
      }
    }

  }
}