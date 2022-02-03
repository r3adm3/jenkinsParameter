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
        sh 'echo $testParameter1 ${params.Greeting}'
      }
    }

  }
}
