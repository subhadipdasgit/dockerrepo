pipeline {
   agent any
stages {
   
   stage('image check'){
        steps{
                sh 'docker images'
             }
        }
   stage('git clone'){
        steps{
               git credentialsId: '7b67be65-92ac-4c3b-9c28-fbbf15a10647', url: 'https://github.com/subhadipdasgit/dockerrepo.git'
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
