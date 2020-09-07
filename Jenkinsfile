#!groovy
//check properties
properties (
  [disableConcurrentBuilds()]
)

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
          sh 'ssh root@docker \'ansible-playbook /etc/ansible/simple.yml\''
      }
    }
  }
}

