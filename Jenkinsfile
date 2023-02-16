pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ working.cpp -o working'
      }
    }
   
    stage('Test') {
      steps {
        sh './working'
      }
    }
   
    stage('Deploy') {
      steps {
        sh ''
      }
    }
  }
 
  post {
    failure {
       
          echo 'Pipeline failed'
        }
    }
   
  }
