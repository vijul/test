pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            sh 'echo "hello world"'
            sh 'echo "hello world"'
          }
        }

        stage('sleep staage') {
          steps {
            sleep 20
          }
        }

      }
    }

    stage('test') {
      steps {
        sleep 10
        git(url: 'https://github.com/vijul/test.git', branch: 'main')
      }
    }

  }
}