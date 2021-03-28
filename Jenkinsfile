pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            when{
                expression{
                  currentBuild.result == null || currentBuild.result == 'SUCCESS'}}
            steps {
                echo 'Deploying....'
                echo ' Environment Details : Build ID=${env.BUILD_ID} on Build Number = ${env.BUILD_NUMBER} with Java Home = ${env.JAVA_HOME} and Jobname= ${env.JOB_NAME and workspace = ${WORKSPACE}}
            }
        }
    }
}
