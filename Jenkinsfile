pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sleep 2
          }
        }
        stage('Stage1a') {
          steps {
            echo 'Stage1a Message'
          }
        }
        stage('Stage1b') {
          steps {
            sleep 3
          }
        }
      }
    }
    stage('Stage2') {
      parallel {
        stage('Stage2') {
          steps {
            echo 'Hello Sage2'
          }
        }
        stage('Stage2b') {
          steps {
            echo 'Stage2b !!!!'
          }
        }
      }
    }
    stage('Stage3') {
      steps {
        echo 'Finished!!!!'
      }
    }
  }
}