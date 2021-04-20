node {
    stage('Checkout SCM') {
        git branch: 'jenkins_test', url: 'https://github.com/ng-mohit/jenkins-test.git'
    }

    stage('Install node modules') {
        sh "npm install"
    }

    stage("Test") {
        sh "npm run test-headless"
    }

    stage("Build") {
        sh "npm run build --prod"
    }
    
    stage("Copy") {
        sh "cp -a C:/Mohit/jenkins-test/dist/jenkins-test/. C:/Mohit/www/jenkins_test/html/"
    }
}