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
        stage('error') {
          steps {
            sh 'echo "hihi"'
          }
        }
      }
    }
    stage('error') {
      steps {
        sh 'echo "abcdefgh"'
      }
    }
  }
}