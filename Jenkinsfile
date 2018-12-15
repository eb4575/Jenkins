pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'cd /home'
          }
        }
        stage('test2') {
          steps {
            echo 'folder changed'
          }
        }
      }
    }
    stage('preproduction') {
      steps {
        echo 'this is pre prod'
      }
    }
  }
}