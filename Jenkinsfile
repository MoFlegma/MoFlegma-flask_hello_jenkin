pipeline {
  agent any
  stages {
    stage('Install dependencies') {
      steps {
        sh 'pip install -r requirements.txt'
        echo 'insallation'
      }
    }

    stage('Run tests') {
      steps {
        sh 'python test.py'
        echo 'test'
      }
    }

    stage('Run application') {
      steps {
        sh 'python app.py'
        echo 'run'
      }
    }

  }
}