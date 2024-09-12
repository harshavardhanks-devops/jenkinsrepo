pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'dev build completed'
          }
        }

        stage('QA') {
          steps {
            echo 'QA build completed'
          }
        }

      }
    }

    stage('Prod') {
      steps {
        echo 'deployed in prod'
      }
    }

  }
}