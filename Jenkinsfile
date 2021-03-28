pipeline {
    agent any
parameters {
  choice choices: ['deveop', '$another'], description: '', name: 'Myproject1'
  gitParameter branch: '', branchFilter: '.*', defaultValue: 'main', description: '', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH_TAG'
}
    stages {
        stage('Example') {
            steps {
                echo "${params.Myproject1} World!"
            }
        }
    }
}
