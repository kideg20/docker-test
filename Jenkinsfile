#!groovy
//check properties
properties (
  [disableConcurrentBuilds()]
)

pipeline {
  agent {
    dockerfile true
    label 'master'
  }
  options {
    timestamps()
  }
  stages {
    stage("DEV") {
      steps {
          sh 'ssh root@docker \'hostname\''
      }
    }
  }
}

