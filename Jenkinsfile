pipeline {
agent any
stages {
   stage('dockerhub login'){
        steps{
           // withCredentials([string(credentialsId: 'dockerpush', variable: 'password')]) {
                   // sh 'docker login -u akashmukh -p $password'
              
            withCredentials([usernameColonPassword(credentialsId: 'pushdocker', usernameVariable: 'user' , passwordVariable: 'pass')]) {
                // some block
              //}
                          sh 'docker login -u $user -p $pass'
                     }
             }
        }
   stage('docker pull'){
        steps{
             sh 'docker pull busybox'
             } 
          }
      }
}
