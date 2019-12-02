pipeline {
  agent {
    docker {
      image 'docker.io/iris/base'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('go version') {
      steps {
        sh 'go --version'
      }
    }

    stage('go run app') {
      steps {
        sh 'go run app.go'
      }
    }

  }
}