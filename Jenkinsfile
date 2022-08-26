
pipeline {
  agent any
  tools{
    maven 'Maven3'
    jdk 'jdk9'
  }
  stages{
    stage("build") {
     
      steps {
        echo 'install the app'
        sh "sh 'mvn -Dmaven.test.failure.ignore=true install'"
      }
    }
    stage("test") {
      steps {
        echo 'testing the app'
      }
    }
    stage("deploy") {
      steps {
        echo "deploying with }"
      }
    }
  }
}
