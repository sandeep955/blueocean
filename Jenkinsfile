pipeline {
  agent any
  stages {
    stage('Checkout') {
      parallel {
        stage('Checkout') {
          steps {
            git(url: 'https://github.com/sandeep955/blueocean.git', branch: 'main')
          }
        }

        stage('') {
          steps {
            echo 'Building'
          }
        }

      }
    }

    stage('') {
      steps {
        echo 'done'
      }
    }

  }
  environment {
    Company = 'Juno'
    Location = 'Hyd'
  }
}