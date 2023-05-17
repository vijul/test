pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        tool(name: 'maven', type: 'testing')
      }
    }

    stage('error') {
      steps {
        sh 'Hello World'
      }
    }

  }
}