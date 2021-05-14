pipeline {
   agent any
stages {
   stage('dockerhub login'){
        steps{
                sh 'docker login -u sayan556 -p Sayanm15@'
             }
   }
   stage('docker pull'){
        steps{
                sh 'docker pull busybox'
             }
   }
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
   stage('image push'){
        steps{
               //1 sh 'docker tag busybox sayan556/busybox:latest'
               sh 'docker tag busybox:latest dock:sayan'
              sh 'docker push sayan556/dock:sayan'

             // 2  sh 'docker push sayan556/busybox:latest'
              //  sh 'docker push sayan556/nginx'
             }
        }
   
      }
}
