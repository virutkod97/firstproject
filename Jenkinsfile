pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Starting Build'
            sh '''chmod +x file
./file'''
          }
        }
        stage('') {
          steps {
            timeout(time: 2)
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'echo "abcdefgh"'
      }
    }
  }
}