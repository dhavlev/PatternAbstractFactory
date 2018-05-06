pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          agent any
          steps {
            sh 'echo "Hi, This is my first build"'
          }
        }
        stage('another shell') {
          steps {
            echo 'Hi this is from another shell'
          }
        }
      }
    }
  }
}