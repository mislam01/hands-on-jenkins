pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test Firefox') {
          steps {
            echo 'Testing'
          }
        }

        stage('Test Chrome') {
          steps {
            echo 'Testing Chrome'
          }
        }

        stage('Test Edge') {
          steps {
            echo 'Testing Edge'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}