pipeline {
   agent any
stages {
   stage('dockerhub login'){
        steps{
                sh 'docker login -u sayan556 -p Sayanm15@'
             }
   }
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
   stage('image push'){
        steps{
                sh 'docker push -a sayan556/test/nginx:latest'
             }
        }
   
      }
}
