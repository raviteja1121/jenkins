pipeline {
  agent any
  stages {
    stage('checgit branch') {
      steps {
        script {
          def scmVars
          scmVars = checkout scm
          echo scmVars.GIT_BRANCH
          sh 'git log -1 --oneline'
        }
      }
    }
  }
}
