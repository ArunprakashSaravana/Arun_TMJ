String branchName = env.Arun
String gitCredentials = "CREDENTIAL_ID"
String repoUrl = "https://github.com/ArunprakashSaravana/Arun_TMJ.git/"

node {
  // Start Stages
  stage('Clone') {
      // Clones the repository from the current branch name
      echo 'Make the output directory'
      sh 'mkdir -p build'

      echo 'Cloning files from (branch: "' + branchName + '" )'
      dir('build') {
          git branch: branchName, credentialsId: 	gitCredentials, url: repoUrl
      }     
  }       
}
