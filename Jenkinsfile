pipeline {
  agent any
  stages {
    stage("Build") {
      steps{
         echo "Hello world!"
         writeFile file: 'test-results.txt', text: 'hello world!'
      }
    }
  }
  post {
    success {
      archiveArtifact 'test-results.txt'
    }
  }
}
