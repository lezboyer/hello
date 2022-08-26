CODE_CHANGES = getGitChanges()
pipeline {
  agent any
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
  }
}
