pipeline{
  agent any
  stages{
    stage('checkout'){
    
        when{
          expression{
            param.Environment == Dev
          }
        }{
      steps {
          git url: 'https://github.com/chaithrab12/Jenkins_CICD',
          branch: 'dev'
        }
      }

       when{
          expression{
            param.Environment == PROD
          }
        }{
      steps {
          git url: 'https://github.com/chaithrab12/Jenkins_CICD',
          branch: 'main'
        }
      }
    }
  

    stage('Build'){
      steps{
        sh 'python3 Test.py'
      }
    }

  }   
}
