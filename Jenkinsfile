pipeline {

agent any

stages {

stage ('Checkout') 
{
steps
    {
    
        checkout scm
        
    }
    
}
stage ('Build') 
{
    steps
    {
       sh "/var/lib/jenkins/workspace/node-hello ; sudo npm install " 
    }
}

   
stage ('Deployment')
    {
    steps
    {
        sh "/var/lib/jenkins/workspace/node-hello; sudo npm start  " 
    }
}
  

}
}
