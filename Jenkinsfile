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
                sh 'docker pull nginx'
             }
   }
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
   stage('image push'){
       steps{
               sh 'docker tag nginx sayan556/dock2:sayan'
               //sh 'docker tag busybox(imagename) sayan556(username)/dock(reponame):sayan(tagname)'
              sh 'docker push sayan556/dock2:sayan'

             }
        }
   
      }
}
