pipeline {
agent any
stages {
   stage('dockerhub login'){
        steps{
           // withCredentials([string(credentialsId: 'dockerpush', variable: 'password')]) {
                   // sh 'docker login -u akashmukh -p $password'
              
            //withCredentials([usernameColonPassword(credentialsId: 'pushdocker', usernameVariable: 'user' , passwordVariable: 'pass')]) {
                // some block
              //}       
               sh 'sudo -S docker login -u sayan556 -p Sayanm15@'
                     //}
             }
        }
   stage('docker pull'){
        steps{
             sh 'docker pull busybox'
             } 
          }
      }
}
