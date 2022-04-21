pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {
     stage('Stop React App') {
      steps {
        bat 'npm stop'
      }
    }   
    stage('Cloning Git') {
      steps {
        git 'https://github.com/GokulNathInfotech/testing.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        bat 'npm install'
      }
    }
     
    stage('Start') {
      steps {
         bat 'npm start'
      }
    }      
  }
}
