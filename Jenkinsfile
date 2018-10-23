pipeline {
  agent {
    kubernetes {
      def label = "worker-${UUID.randomUUID().toString()}"
      label label
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
