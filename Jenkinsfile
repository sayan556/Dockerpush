pipeline {
   agent{
      docker { image 'nginx:latest' }
   }
stages {
   stage('dockerhub login'){
        steps{
                sh 'docker login -u sayan556 -p Sayanm15@'
             }
        }
   
      }
}
