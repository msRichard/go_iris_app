pipeline {
  agent {
    docker {
      image 'golang'
    }

  }
  stages {
    stage('go run app') {
      steps {
        sh 'cd ../go_iris_app_master'
        sh 'go run app.go'
      }
    }

  }
}