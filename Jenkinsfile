pipeline {
   agent any
stages {
   
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
   
   //stage('image pull'){
        //steps{
                //sh 'docker pull subhadipdocker/subhadip:latest'
             
             //}
        //}
   //stage('dockerhub login'){
        //steps{
                //sh 'docker login -u subhadipdocker -p 7699676975'
             //}
        //}
   //stage('image push'){
       //steps{ 
            //sh 'docker tag nginx subhadipdocker/subhadip:latest'
            //sh 'docker push subhadipdocker/subhadip:latest'
            //}
       //}
   stage('deployment'){
        steps{
                sh 'kubectl apply -f nginxjenkins.yml'
                sh 'kubectl get all'
             
             }
        }
    } 
}
