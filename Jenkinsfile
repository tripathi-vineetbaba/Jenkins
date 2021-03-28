pipeline {
    agent any
    parameters {
        choices('Jenkins', 'Jenkins-1', 'Jenkins-2', description: '''Select any 1 repo from these 3:
          Jenkins
          Jenkins-Temp
          Jenkins-Temp2''', name: 'Jenkins Repo')
    }
    stages {
        stage('Example') {
            steps {
                echo "${params.Greeting} World!"
            }
        }
    }
}
