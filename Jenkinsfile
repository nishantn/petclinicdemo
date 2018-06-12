pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/nishantn/petclinicdemo.git', branch: 'master', poll: true)
      }
    }
  }
}