pipeline{
  agent any
  stages{
    stage('checkout'){
      steps {
        git url: 'https://github.com/chaithrab12/Jenkins_CICD',
        branch: 'main'
      }
    }

    stage('Build'){
      steps{
        python3 test.py
      }
    }

    
  }
  
}
