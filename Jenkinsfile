pipeline {
    agent {
      label 'test5linux'
    }

    stages {
    stage('maven install') {
      steps {
        withMaven(maven: 'Maven3') {
        sh 'mvn clean install'
}
      }
    }

  }


}
