pipeline {
   agent{
      docker { image 'nginx:latest' }
   }
stages {
   stage('dockerhub login'){
        steps{
                sh 'docker nginx --version'
             }
        }
   
      }
}
