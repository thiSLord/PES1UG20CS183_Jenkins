pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o Pipeline_183 Pipeline_183.cpp'
        build job: 'PES1UG20CS183-1'
        echo 'Build stage successful'
      }
    }
    stage('Test') {
      steps {
        sh './Pipeline_18'
        echo 'Test stage successful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy stage successful'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
      
    
    
