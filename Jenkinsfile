pipeline {
  agent any
  stages {
    stage('Prepare Image') {
      steps {
        sh 'bash ./jenkins/scripts/prepare-image.sh'
      }
    }
  }
  environment {
    HOME = '.'
    DOCKER_HUB_USER = 'saransasidharan'
    DOCKER_HUB_PASSWORD = '@swasar007rek'
    CONTAINER_PORT = '9090'
    HOST_PORT = '9090'
    DB_CONN_STRING = 'ZGF0YSBzb3VyY2U9aW9tZWdhc3Fsc2VydmVydjIuZGF0YWJhc2Uud2luZG93cy5uZXQ7dXNlciBpZD1pb21lZ2FhZG1pbjtwYXNzd29yZD1QcmVzdGlnZTEyMztpbml0aWFsIGNhdGFsb2c9aW9tZWdhc3FsZGF0YWJhc2V2Mjs='
    CONTAINER_NAME = 'restservices'
    CLUSTER_NAME = 'saran-cluster'
  }
}