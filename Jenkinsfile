pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                echo "This is build step in DEV1."
                echo "Ensuring multiline login in build step"
            }
                    }
        stage('test'){
            steps{
                echo "This is testing step  in DEV1."
                echo "Ensuring multiline comment in testing"
            }
        }
        stage('deploy'){
            steps{
                echo "This is deploy stage  in DEV1."
                echo "Ensuring multiline comment in testing"
            }
        }
    }
}
