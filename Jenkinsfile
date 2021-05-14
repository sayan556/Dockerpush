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
               sh 'docker tag busybox sayan556/dock:sayan'
               //sh 'docker tag busybox(imagename) sayan556(username)/dock(reponame):sayan(tagname)'
              sh 'docker push sayan556/dock:sayan'

             }
        }
   
      }
}
