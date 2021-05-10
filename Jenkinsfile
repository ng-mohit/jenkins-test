pipeline {
   agent any
      environment {
         PATH='C:/Program Files/Git/bin;C:/Program Files/nodejs/;C:/Users/devteam/AppData/Roaming/npm'
      }
   stages {
      stage('NPM Setup') {
      steps {
         sh 'npm install'
      }
   }

   stage('Angular Build') {
   steps {
      sh 'npm run build --prod'
     } 
  }

   stage('Angular Test Build') {
   steps {
      sh 'ng test'
   }
  }

 }
}