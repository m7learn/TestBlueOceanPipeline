pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Best DevOps'
      }
    }

    stage('Test 1') {
      parallel {
        stage('Test 1') {
          steps {
            echo 'ok Test 1'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Ok test 2'
          }
        }

      }
    }

    stage('Deploy ') {
      steps {
        input(message: 'are you to Deploy ', ok: 'yes')
        echo 'ok done Deploy '
      }
    }

  }
}