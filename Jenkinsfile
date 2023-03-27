pipeline {
  agent any
  tools {
    nodejs '19.8.1'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Install dependencies') {
      steps {
        sh 'npm init'
      }
    }
    stage('Run tests') {
      steps {
        sh 'npm test'
      }
    }
  }
}