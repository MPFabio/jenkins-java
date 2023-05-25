pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        sh "rm -rf *"
        sh "git clone https://github.com/MPFabio/jenkins-java"
      }
    }
    stage('compile') {
      steps {
        sh "cd jenkins-java/ && javac Main.java"
      }
    }
   stage('run') {
      steps {
        sh "cd jenkins-java/ && java Main"
      }
    }
  }
}
