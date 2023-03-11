pipeline {
  agent any
  stages {
    stage('for main branch') {
      when {
        branch 'main'
      }
      steps {
        echo 'main branch'
      }
    }
    stage('for stage branch') {
      when {
        branch 'stage'
      }
      steps {
        echo 'stage branch'
      }
    }
/*    stage('for dev branch') {
      when {
        branch 'dev'
      }
      steps {
        echo 'dev branch'
      }
    }*/       
    stage('for pull request') {
      when {
        changeRequest()
      }
      steps {
        echo 'pull request'
      }
    }
  }
}
