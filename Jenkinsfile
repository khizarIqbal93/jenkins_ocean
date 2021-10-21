pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'hello'
        sh 'echo "second step"'
        sleep 1
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

    stage('Deploy') {
      steps {
        sh 'echo "deploying"'
      }
    }

  }
}