pipeline {
  agent any
  stages {
    stage('Install dependencies') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }

    stage('Run tests') {
      steps {
        sh 'python test.py'
      }
    }

    stage('Run application') {
      steps {
        sh 'python app.py'
      }
    }

  }
}