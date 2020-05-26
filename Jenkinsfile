pipeline {
  agent any
  stages {
    stage('step1') {
      steps {
        echo 'allo'
        sleep 10
      }
    }

    stage('step2') {
      parallel {
        stage('step2') {
          steps {
            echo 'tsts'
            sleep 15
          }
        }

        stage('bbbblblblazzzzzz') {
          steps {
            sleep 30
            sh 'echo `date`'
          }
        }

      }
    }

    stage('step3') {
      parallel {
        stage('step3') {
          steps {
            build 'cmd2rest'
          }
        }

        stage('echo patate') {
          steps {
            sh 'echo patate'
          }
        }

      }
    }

  }
  environment {
    ALLO = 'yobitch'
  }
}