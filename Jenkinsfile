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
   stage('dockerhub login'){
        steps{
                sh 'docker login -u subhadipdocker -p 7699676975'
             }
        }
   stage('image push'){
       steps{ 
            sh 'docker tag nginx subhadipdocker/subhadip:exam'
            sh 'docker push subhadipdocker/subhadip:exam'
            }
       }
   } 
}
