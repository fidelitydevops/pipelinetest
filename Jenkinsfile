pipeline {
    agent {
        label 'javavm'
    }
    environment {
        var1 = "value1"
    }
    stages {
        stage('clonethecode') {
            steps {
                git 'https://github.com/fidelitydevops/testprojectone'
            }
        }
        stage('build') {
            steps {
                sh 'echo two'
            }
        }
        stage('execute test') {
            steps {
                sh 'echo three'
            }
        }
        stage('approval') {
            steps {
                input 'Approved to Deploy ?'
            }
        }
        stage('deploy') {
            steps {
                sh 'echo deploy'
            }
        }
        
    }
}
