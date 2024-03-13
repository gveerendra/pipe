pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'Dev'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Test'
          }
        }

        stage('prod') {
          steps {
            echo 'prod'
          }
        }

        stage('dep') {
          steps {
            echo 'Dep'
          }
        }

      }
    }

  }
}