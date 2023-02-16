pipeline {
  agent any
	
  stages {
    stage('build') {
      steps {
        sh 'g++ working.cpp -o working'
      }
    }
	
    
    stage('test') {
      steps {
        sh './working'
        echo 'final output'
      }
    }
    
	
    stage('deploy') {
      steps {
	echo 'deploying'
      }
    }
  }
  
  post {
    failure {
      echo 'pipeline isnt successful'
       }
    }
  }
}
