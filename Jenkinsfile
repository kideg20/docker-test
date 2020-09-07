#!groovy
//check properties
properties (
  [disableConcurrentBuilds()]
)

pipeline {
  agent {
    dockerfile true
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

