pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh ' sudo npm install'
      }
    }
     
    stage('Deployment') {
      steps {
         sh 'sudo npm start '
      }
    }      
  }
}
