pipeline {
    agent any
parameters {
  choice choices: ['deveop', '$another'], description: '', name: 'Myproject1'
  gitParameter branch: '', branchFilter: '.*', defaultValue: 'main', description: '', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH_TAG'
      checkboxParameter name:'mycheckbox', format:'JSON', uri:'https://raw.githubusercontent.com/sunweisheng/Jenkins/master/examples/example.json'
}
    stages {
        stage('Example') {
            steps {
                echo "${params.Myproject1} World!"
                echo "${params.mycheckbox}"
            }
        }
    }
}
