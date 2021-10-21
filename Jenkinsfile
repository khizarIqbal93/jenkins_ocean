pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'hello'
      }
    }

    stage('Test') {
      steps {
        sh '''echo "test running"
python --version'''
      }
    }

  }
}