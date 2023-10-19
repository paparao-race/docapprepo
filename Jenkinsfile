pipeline {
  agent any
  stages {
    stage('buildStage') {
      steps {
        sh '''sudo docker login -u paparaorace -p "dckr_pat_AtW6ulytniwOCOCb8bn9H5FV4NY"
sudo docker build -t paparaorace/myrepo2:${BUILD_NUMBER}  .
sudo docker push paparaorace/myrepo2:${BUILD_NUMBER}'''
      }
    }

  }
}