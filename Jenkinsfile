#!groovy
//check properties
properties ([disableConcurrentBuilds()])

pipeline {
  agent {
    label 'master'
  }
  options {
    timestamps()
  }
  stages {
    stage("DEV") {
      steps {
          sh 'ssh root@docker2 \'hostname\''
      }
    }
  }
}
