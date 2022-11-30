pipeline {
   agent any
   stages {
    stage('Checkout') {
      steps {
        script {
           // The below will clone your repo and will be checked out to master branch by default.
           git credentialsId: 'jenkins-user-github', url: 'https://github.com/ArunprakashSaravana/Arun_TMJ.git'
           sh "git status*" 
           // List git logs. 
           sh "git log"
          }
       }
    }
  }
}
