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
            echo "Current Environment is ${env2}"
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
  environment {
    env2 = 'DEMO'
  }
}
