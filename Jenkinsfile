pipeline {
  agent any

  stages {
  
 
    stage('build') {
      steps {
        sh 'g++ working.cpp -o working.cpp'
      }
    }
	
    
    stage('test') {
      steps {
        sh './working.cpp'
        echo'final output'
      }
    }
    
	
    stage('deploy') {
      steps {
      }
    }
  }
  
  
  post {
    failure {
      echo 'pipeline isnt successful'
    }
  }
}
