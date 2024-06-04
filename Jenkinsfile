pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'teststep'
          }
        }

        stage('testpar') {
          steps {
            echo 'testpar'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'dep'
      }
    }

  }
}