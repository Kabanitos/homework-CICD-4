pipeline {
    agent {
  label 'ansible'
    }
    stages {
        stage ('clone project') {
            steps {
                git branch: 'main', url: 'https://github.com/Kabanitos/homework-CICD-4.git'
            }
        }
        stage ('test molecule'){
            steps {
                sh 'molecule test'
            }
        }