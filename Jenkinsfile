pipeline {
   agent any
stages {
   
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
   stage('image pull'){
        steps{
                sh 'docker pull nginx:latest'
             
             }
        }
   
      }
}
