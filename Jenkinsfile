pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'hello'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh '''echo "test running"
python --version'''
          }
        }

        stage('test1') {
          steps {
            echo 'testing 1'
          }
        }

      }
    }

  }
}