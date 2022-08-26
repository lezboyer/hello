CODE_CHANGES = getGitChanges()
pipeline {
  agent any
  environment {
    SERVER_CREDENTIALS = credentials('jenkins-exemple-private-pat')
  }
  stages{
    stage("build") {
      when {
        expression {
          BRANCH_NAME == 'main' && CODE_CHANGES == true
        }
      }
      steps {
        echo 'building the app'
      }
    }
    stage("test") {
      steps {
        echo 'testing the app'
      }
    }
    stage("deploy") {
      steps {
        echo "deploying with ${SERVER_CREDENTIALS}"
      }
    }
  }
}
