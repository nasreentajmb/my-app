pipeline {
  agent any
  stages{
    stage('SCM checkout'){
      git '
    stage("Maven Build"){
      steps{
        def mvnHome=tool name: 'Maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn clean package"
      }
    }
  }
}
