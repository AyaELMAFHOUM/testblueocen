pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build-completed'
      }
    }

    stage('test') {
      parallel {
        stage('test1') {
          steps {
            echo 'test-completed'
          }
        }

        stage('test 2') {
          steps {
            echo 'test2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy-completed'
      }
    }

  }
}