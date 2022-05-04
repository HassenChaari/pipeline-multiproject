pipeline {
  agent any
  stages {
    stage('init') {
      steps {
        sh 'echo "init"'
      }
    }

    stage('Base-step1') {
      parallel {
        stage('Base-step1') {
          steps {
            sh 'echo "base-init"'
          }
        }

        stage('P02-step1') {
          steps {
            sh 'echo "P02-step1"'
          }
        }

        stage('P03-step2') {
          steps {
            sh 'echo "P03-step2"'
          }
        }

      }
    }

    stage('Base-step2') {
      parallel {
        stage('Base-step2') {
          steps {
            sh 'echo "base-step2"'
          }
        }

        stage('P02-step2') {
          steps {
            sh 'echo "P02-step2"'
          }
        }

        stage('P03-step2') {
          steps {
            sh 'echo "P03-step2"'
          }
        }

      }
    }

    stage('base-finish') {
      steps {
        sh 'echo "finish" '
      }
    }
  }
}
