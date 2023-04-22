pipeline {
  agent any
  stages {
    stage('checgit branch') {
      steps {
        script {
          def scmVars
          scmVars = checkout scm
          echo scmVars.GIT_BRANCH
          def commit = sh(returnStdout: true, script: 'git log -1 --oneline | grep -i '^\#*$ '').trim()
          echo "$commit"
        }
      }
    }
  }
}
