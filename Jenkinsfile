pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'npm install'
        sh 'npm run build'
      }
    }

    stage('test') {
      steps {
        sh 'npm install'
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        sh 'npm install'
        sh 'npm run package'
      }
    }

  }
  tools {
    nodejs 'NodeJS 4.8.6'
  }
}