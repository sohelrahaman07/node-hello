pipeline {
agent {
label 'master'
}

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
       sh "cd /var/lib/jenkins/workspace/NodeHelloJob ; sudo npm install " 
    }
}

   
stage ('Deployment')
    {
    steps
    {
        sh "/var/lib/jenkins/workspace/NodeHelloJob ; sudo npm start  " 
    }
}
  

}
}
