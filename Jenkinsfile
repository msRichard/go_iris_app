pipeline {
  agent {
    docker {
      image 'docker.io/iris/base'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('go run app') {
      steps {
        sh 'go run app.go'
      }
    }

  }
}