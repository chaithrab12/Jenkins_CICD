pipeline{
  agent any
  stages{
    stage('checkout'){
    
      steps {
          git url: 'https://github.com/chaithrab12/Jenkins_CICD',
          branch: "${params.Environment}"
        }
    
    stage('Build'){
      steps{
        sh 'python3 Test.py'
      }
    }

  }   
}
