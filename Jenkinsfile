pipeline {
  agent any
  stages {
    stage('checkgit branch') {
      steps {
        script {
          def GIT_BRANCH=sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
          echo "$GIT_BRANCH"
        }
      }
    }
  }
}
