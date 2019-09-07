pipeline {
  agent any
  stages {
    stage('build job1') {
      steps {
        build(job: 'test', quietPeriod: 3)
        sh '''pipeline {
    agent any 

    stages {
        stage(\'Build Assets\') {
            agent any 
            steps {
                echo \'Building Assets\'
            }
        }
        stage(\'Test\') {
            agent any
            steps {
                echo \'Testing stuff...\'
            }
        }
    }
}'''
        }
      }
      stage('build job2') {
        steps {
          echo 'Hi hello'
        }
      }
    }
  }