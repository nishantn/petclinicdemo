pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            git(url: 'https://github.com/nishantn/petclinicdemo.git', branch: 'master', poll: true)
            sh 'echo "In Build"'
          }
        }
        stage('Test') {
          steps {
            sh 'echo "In Test"'
          }
        }
      }
    }
    stage('Deploy in QA') {
      steps {
        sh 'echo "In Deploy"'
      }
    }
  }
}