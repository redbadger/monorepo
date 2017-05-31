pipeline {
  agent any
  stages {
    stage('Build') {
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
    stage('Test') {
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
    stage('Deploy') {
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
