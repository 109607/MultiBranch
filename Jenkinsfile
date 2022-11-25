#!groovy
@Library(value="jenkins_pipeline_lib", changelog=false) _





pipeline{
  agent any
  stages{
    stage('hello'){
      steps{
	script {
        version(1.2.3)
        sh 'echo Hello World'
      }
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
