pipeline{
  agent any
  stages{
    stage('hello'){
      steps{
        sh 'echo Hello World'
      }

    }
    stage('Condition'){
    when {
      branch "main"
    }
    steps{
     sh '''
        cat README.md

	'''
    }

    }
  }
}
