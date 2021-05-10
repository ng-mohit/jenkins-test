pipeline {
   agent any
      environment {
         PATH='C:/Windows/System32;C:/Program Files/nodejs/;C:/Users/devteam/AppData/Roaming/npm'
      }
   stages {
      stage('NPM Setup') {
      steps {
         bat 'npm install'
      }
   }

   stage('Angular Build') {
   steps {
      bat 'npm run build --prod'
     } 
  }

   stage('Angular Test Build') {
   steps {
      bat 'ng test'
   }
  }

 }
}