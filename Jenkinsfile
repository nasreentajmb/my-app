pipeline {
  agent any
  stages{
    stage('SCM checkout'){
      git 'https://github.com/nasreentajmb/my-app.git'
    }
    stage("Maven Build"){
      steps{
        def mvnHome=tool name: 'Maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
      }
    }
  }
}
