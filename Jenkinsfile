pipeline{
  agent any
  stages{
    stage('Build app'){
      steps{
        checkout scmGit(branches:[[name: '*/main']],extensions:[],userRemoteConfigs:[[url:'https://github.com/Rashmi-2002/Dockerize']])
      }
    }
    stage('Build docker image'){
      steps{
         script{
           bat 'docker build -t jenkinsjavaapp .'
         }
        
      }
    }
  }
}
