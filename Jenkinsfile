pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/sohelrahaman07/node-hello.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'sudo npm install'
      }
    }
     
    stage('Deployment') {
      steps {
         sh 'sudo npm start'
      }
    }      
  }
}
