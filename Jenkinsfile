pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is devopment stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'this is test stage'
          }
        }

        stage('build') {
          steps {
            echo 'this is build stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deployment stage'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate'
          }
        }

      }
    }

  }
}