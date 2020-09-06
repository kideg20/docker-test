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
    stage("Log in to docker") {
      steps {
        step {
          sh 'ssh root@docker \'hostname\''
        }
      }
    }
  }
}
