#!groovy
//check properties
properties (
  [disableConcurrentBuilds()],
  [pipelineTriggers([githubPush()])]
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
          sh 'ssh root@docker \'hostname\''
      }
    }
  }
}
