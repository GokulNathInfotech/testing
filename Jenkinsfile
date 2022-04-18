pipeline {
  agent any
    
  tools {nodejs}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/GokulNathInfotech/testing.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh '<<Build Command>>'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}