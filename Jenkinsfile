pipeline {
    agent {
      label 'test5linux'
    }
    
    stages {
    stage('Build') {

            **dir('project-dir') {**
                sh 'mvn clean install'

                def pom = readMavenPom file:'pom.xml'

                print pom.version
                env.version = pom.version
            }
    }

  }

  
}
