pipeline {
  agent any
  stages {
    stage('') {
      steps {
        parallel(
          "API Build": {
            echo 'Building API...'
            
          },
          "Web Build": {
            echo 'Building Web...'
            
          }
        )
      }
    }
    stage('API Test') {
      steps {
        parallel(
          "API Test": {
            echo 'Testing API...'
            
          },
          "Web Test": {
            echo 'Testing Web...'
            
          }
        )
      }
    }
    stage('API Deploy') {
      steps {
        parallel(
          "API Deploy": {
            echo 'Deploying API...'
            
          },
          "Web Deploy": {
            echo 'Deploying Web...'
            
          }
        )
      }
    }
  }
}