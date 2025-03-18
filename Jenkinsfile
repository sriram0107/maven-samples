pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/sriram0107/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
  tools {
    maven 'DHT_MVN'
    jdk 'DHT_SENSE'
  }
}
