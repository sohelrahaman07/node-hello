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
       sh "cd /home/ubuntu/workspace/MONOANGULARJOB ; sudo npm install " 
    }
}

   
stage ('Deployment')
    {
    steps
    {
        sh "cd /home/ubuntu/workspace/MONOANGULARJOB ; sudo npm start  " 
    }
}
  

}
}
