pipeline {
  agent {
    kubernetes {
      label 'mypodtemplate-npm-6-l2dqd-w6b4k'
      defaultContainer 'node-container'
      yamlFile 'KubernetesPod.yaml'
    }
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}
