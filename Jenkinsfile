pipeline {
    agent any
parameters {
  choice choices: ['deveop', '$another'], description: '', name: 'Myproject1'
}
    }
    stages {
        stage('Example') {
            steps {
                echo "${params.Greeting} World!"
            }
        }
    }
}
