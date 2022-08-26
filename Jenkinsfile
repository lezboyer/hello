
pipeline {
  agent any
  tools{
    maven 'Maven3'
    jdk 'jdk9'
  }
  stages{
    stage ('Initialize') {
      steps {
          sh '''
              echo "PATH = ${PATH}"
              echo "M2_HOME = ${M2_HOME}"
          ''' 
      }
    }
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
