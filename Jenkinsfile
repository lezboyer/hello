
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
        sh "mvn install"
      }
      steps {
        echo 'building the app'
        sh "mvn install"       
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
