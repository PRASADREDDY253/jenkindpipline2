pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is build stage'
          }
        }

        stage('Test') {
          steps {
            echo 'This is testing phase'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'This is deploy stage'
      }
    }

  }
}