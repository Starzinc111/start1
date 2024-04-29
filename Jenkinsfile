pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "2+1"'
      }
    }

    stage('Test') {
      parallel {
        stage('Test Front') {
          steps {
            echo 'Frontend'
          }
        }

        stage('Test Back') {
          steps {
            echo 'Backend'
          }
        }

      }
    }

  }
}