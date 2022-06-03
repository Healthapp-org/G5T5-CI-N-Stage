pipeline {
  agent any
  stages {
    stage('Git checkout'){
      steps{
        git branch: 'main', credentialsId: 'f7c765a1-e95f-44ad-9f53-7b9fc6ad20ec', url: 'https://github.com/Healthapp-org/G5T5-CI-N-Stage.git'
      }
    }
  }
}
