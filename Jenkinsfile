pipeline {
  agent any
  stages {
    stage('checkgit branch') {
      steps {
        script {
          def scmVars
          scmVars = checkout scm
          echo scmVars.GIT_BRANCH
        }
      }
    }
  }
}
