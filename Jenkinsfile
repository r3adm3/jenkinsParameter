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
        echo "Hello ${params.FirstName}!" > /tmp/doodad.txt
        sh 'echo $testParameter1'
      }
    }

  }
}
