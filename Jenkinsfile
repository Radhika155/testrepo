pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'dev stage'
      }
    }

    stage('dev') {
      parallel {
        stage('dev') {
          steps {
            echo 'dev stage'
          }
        }

        stage('qa') {
          steps {
            echo 'qa stage'
          }
        }

      }
    }

    stage('prod') {
      steps {
        echo 'prod stage'
      }
    }

  }
}