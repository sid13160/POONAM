pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat 'cd'
        echo 'BUILD'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing'
          }
        }

        stage('parallel_test') {
          steps {
            echo 'parallel testing'
          }
        }

      }
    }

    stage('prod') {
      steps {
        echo 'Production'
      }
    }

  }
}