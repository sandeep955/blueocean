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

        stage('Print1') {
          steps {
            echo 'Building'
          }
        }

      }
    }

    stage('Print2') {
      steps {
        echo 'done'
      }
    }

    stage('Print3') {
      steps {
        echo "My Company ${Company}"
      }
    }

  }
  environment {
    Company = 'Juno'
    Location = 'Hyd'
  }
}
