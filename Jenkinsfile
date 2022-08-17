node {
      stage('SCM checkout'){
          git 'https://github.com/nasreentajmb/my-app.git'
       }
      stage("Maven Build"){
        def mvnHome = tool name: 'Maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
      }
}
