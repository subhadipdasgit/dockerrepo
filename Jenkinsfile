pipeline {
   agent any
stages {
   stage('dockerhub login'){
        steps{
                sh 'docker login -u subhadipdocker -p 7699676975'
             }
   }
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
