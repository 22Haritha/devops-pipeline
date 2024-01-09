pipeline {
  agent any
  stages {
    stage('commit') {
      steps {
        echo 'commit the code'
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

        stage('Stage') {
          steps {
            echo 'stage the code'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the code'
          }
        }

        stage('Operate') {
          steps {
            echo 'operate the app'
          }
        }

      }
    }

  }
}