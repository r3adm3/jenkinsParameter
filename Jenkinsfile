pipeline {
  agent any
  parameters {
        string(name: 'FirstName', defaultValue: 'Person', description: 'How should I greet the world?')
    }
  stages {
    stage('First Stage') {
      environment {
        testParameter1 = 'doodad'
      }
      steps {
        echo "Hello ${params.FirstName}!"
        whoami
        sh 'echo $testParameter1'
      }
    }

  }
}
