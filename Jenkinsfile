pipeline {
    agent any
    triggers {
  pollSCM('* * * * *')
    }
    stages {
        stage("create zip file"){
            steps{
                sh 'zip crudcode-pipeline-${BUILD_NUMBER}.zip * --exclude Jenkinsfile'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello '
                sleep 5
            }
        }
          stage('build') {
            steps {
                echo 'build'
                sleep 5
            }
        }
          stage('test') {
            steps {
                echo 'test'
                sleep 5
            }
        }
          stage('deploy') {
            steps {
                echo 'deploy'
                sleep 4
            }
        }
    }
}