pipeline {
  agent any
  stages {
    stage('stage 1') {
      parallel {
        stage('stage 1') {
          steps {
            echo 'stage 1. Hello'
          }
        }

        stage('stage2') {
          steps {
            sleep(unit: 'NANOSECONDS', time: 100)
          }
        }

      }
    }

    stage('stage4') {
      steps {
        git(url: 'https://github.com/waterwaterwater/bfuse.git', branch: 'master')
      }
    }

  }
  environment {
    second = '2'
  }
}