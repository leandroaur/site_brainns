pipeline {
  agent any
  stages {
    stage('Build our website') {
      steps {
        sh "scripts/build.sh"
      }
    }

    stage('Run unit tests') {
      steps {
        sh "scripts/unit_tests.sh"
      }
    }

    stage('Deloy website') {
      steps {
        sh "scripts/deploy_website.sh"
      }
    }
  }
}
