pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o PES1UG22CS443-1 main.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test') {
      steps {
        sh './PES1UG22CS443-1'
        echo 'Test Stage Successful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying Application'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
    
