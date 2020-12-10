pipeline {
  agent any
  stages {
    stage("Build") {
      steps {
         echo "Hello world!"
         writeFile file: 'test-results.txt', text: 'hello world!'
      }
      steps {
        sh 'ls -htl'
        sh 'echo listing all files'
      }    
    }
  }
  post {
    success {
      archiveArtifacts 'test-results.txt'
    }
  }
}
