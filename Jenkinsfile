// node {
//     stage('Checkout SCM') {
//         git branch: 'jenkins_test', url: 'https://github.com/ng-mohit/jenkins-test.git'
//     }

//     stage('Install node modules') {
//         sh "npm install"
//     }

//     stage("Test") {
//         sh "npm run test-headless"
//     }

//     stage("Build") {
//         sh "npm run build --prod"
//     }
    
//     stage("Copy") {
//         sh "cp -a C:/Mohit/jenkins-test/dist/jenkins-test/. C:/Mohit/www/jenkins_test/html/"
//     }
// }

pipeline {
   agent any
      environment {
         PATH='C:/Program Files/nodejs/;C:/Users/devteam/AppData/Roaming/npm'
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

//    stage('APK Sign') {
//    steps {
//       sh 'jarsigner -storepass your_password -keystore keys/yourkey.keystore platforms/android/app/build/outputs/apk/release/app-release-unsigned.apk nameApp'
//    }
//    }

//    stage('Stage Web Build') {
//       steps {
//         sh 'npm run build --prod'
//     }
//   }

//    stage('Publish Firebase Web') {
//       steps {
//       sh 'firebase deploy --token "Your Token Key"'
//    }
//   }

   //stage('Publish iOS') {
//       steps {
//        echo "Publish iOS Action"
//     }
//    }

//    stage('Publish Android') {
//      steps {
//     echo "Publish Android API Action"
//    }
//   }

 }
}