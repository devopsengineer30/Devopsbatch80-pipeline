pipeline {
  agent any
  stages {
    stage('commit') {
      steps {
        echo 'Commit the code'
      }
    }

    stage('Build') {
      steps {
        echo 'Build the code'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test the code'
          }
        }

        stage('stage') {
          steps {
            echo 'stage the code'
          }
        }

        stage('deploy') {
          steps {
            echo 'Deploy the code'
          }
        }

        stage('Operate') {
          steps {
            echo 'Operate the app'
          }
        }

      }
    }

  }
}