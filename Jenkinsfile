
pipeline {
  agent any
  tools{
    maven 'Maven3'
  }
  stages{
  
    stage("build") {
     
      steps {
        echo 'install the app'
        sh 'mvn -Dmaven.test.failure.ignore=true install'
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
