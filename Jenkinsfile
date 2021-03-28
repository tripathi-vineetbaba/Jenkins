pipeline {
  agent any
  parameters {
    gitParameter(branch: '', branchFilter: '.*', defaultValue: 'dev1', description: '', name: 'BRANCH')
  }
  stages {
    stage('Example') {
      steps {
        sh('echo ${STATEMENT}')
      }
    }
  }
}
