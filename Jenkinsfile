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
         rmdir file
         mkdir file
         ls -ltr
         '''
          sh 'rmdir timeoutfile'
        }
        timeout(time: 20, unit: 'SECONDS'){
          
          sh 'sleep 40'
          sh 'mkdir timeoutfile'
          sh 'ls -ltr'
        }
    
    }
                   }
  }
}
post {
  always{
  echo 'This is always run post parameter'
  }
  changed{
  echo "This is expected to run this time as build status is changed"
  }
  success{
  echo "This nuild is successfull"
  }
  failure{
    echo "This is failed build"
}
}
