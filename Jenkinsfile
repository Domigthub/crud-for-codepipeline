pipeline {
    agent any
    triggers {
  pollSCM('* * * * *')
    }
    stages {
        stage("create zip file"){
            steps{
              sh  'zip crudcode-${BUILD_NUMBER}.zip * --exclude Jenkinsfile'
            }
        }
    }
}