pipeline {
  agent any
  parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
  stages {
    stage('First Stage') {
      environment {
        testParameter1 = 'doodad'
      }
      steps {
        echo '${params.Greeting} Adrian'
        sh 'echo $testParameter1'
      }
    }

  }
}
