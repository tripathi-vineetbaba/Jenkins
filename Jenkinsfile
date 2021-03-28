pipeline {
    agent any
    environment{
    BUILD_VARIABLE = 'Build Env Variable'
    TEST_VARIABLE = 'Test Env Variable'
    DEPLOY_VARIABLE = 'Deploy Env Variable'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'Env Variable : $BUILD_VARIABLE'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo 'Env Variable : $TEST_VARIABLE'
            }
        }
        stage('Deploy') {
            when{
                expression{
                  currentBuild.result == null || currentBuild.result == 'SUCCESS' }
            }
            steps {
                echo 'Deploying....'
                echo 'Env Variable : $DEPLOY_VARIABLE' 
                echo ' Environment Details : Build ID=${env.BUILD_ID} on Build Number = ${env.BUILD_NUMBER} with Java Home = ${env.JAVA_HOME} and Jobname= ${env.JOB_NAME} and workspace = ${env.WORKSPACE} '
            }
            }
        }
    }
