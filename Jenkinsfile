pipeline {
   agent docker{
      docker { image 'nginx' }
   }
stages {
   stage('dockerhub login'){
        steps{
                sh 'nginx --version'
             }
        }
   
      }
}
