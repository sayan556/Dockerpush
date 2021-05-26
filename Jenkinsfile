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
                sh 'docker pull sayan556/dock2:sayan'
             }
   }
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
    stage('Git Clone yml file') {
       steps {
// Get some code from a GitHub repository
           git branch: 'main', credentialsId: 'githubcred', url: 'https://github.com/sayan556/Dockerpush.git'
         }
       }
  // stage('Run yml file') {
      // steps {
        //  sh 'kubectl apply -f nginx.yaml'
        //  sh 'kubectl get all'

       //  }
      // }
   stage('image push'){
       steps{
               sh 'docker tag nginx sayan556/dock2:sayan'
               //sh 'docker tag busybox(imagename) sayan556(username)/dock(reponame):sayan(tagname)'
              sh 'docker push sayan556/dock2:sayan'

             }
       }
   
      }
}
