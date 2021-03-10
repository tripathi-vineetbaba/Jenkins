pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                echo "This is build step."
                echo "Ensuring multiline login in build step"
            }
                    }
        stage('test'){
            steps{
                echo "This is testing step"
                echo "Ensuring multiline comment in testing"
            }
        }
        stage('deploy'){
            steps{
                echo "This is deploy stage"
                echo "Ensuring multiline comment in testing"
            }
        }
    }
}
