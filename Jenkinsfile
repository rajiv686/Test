pipeline {
  agent any
  stages {
    stage('build job1') {
      steps {
        build(job: 'test', quietPeriod: 3)
      }
    }
    stage('build job2') {
      steps {
        echo 'Hi hello'
      }
    }
  }
}