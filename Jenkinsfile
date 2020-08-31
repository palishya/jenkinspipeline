pipeline {
    agent any

    stages {
        stage('SCM') {
            steps {
                git credentialsId: 'git', url: 'https://github.com/palishya/jenkinspipeline.git'
            }
        }
        stage('Maven Build') {
            steps {
                sh label: '', script: 'mvn clean'
                sh label: '', script: 'mvn install'
            }
        }
    }
}
