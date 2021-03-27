pipeline{
  agent any
  stages{
    stage('Build From Jenkins Documentation'){
      steps{
        sh 'echo Hello World'
        sh '''
        echo Multiline shell script works too
        ls -ltr
        '''
      }
    }
    stage('Deploy'){
      steps{
        retry(3){
         sh '''
         mkdir file
         ls -ltr
         '''
        }
        timeout(time: 20, unit: 'SECONDS'){
          sh 'mkdir timeoutfile'
          sh 'ls -ltr'
        }
    
    }
                   }
  }
}
