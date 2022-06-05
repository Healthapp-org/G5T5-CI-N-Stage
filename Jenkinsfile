pipeline{
        agent any 
        stages{
          stage('1-gitclone'){
            steps{
              checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'f7c765a1-e95f-44ad-9f53-7b9fc6ad20ec', url: 'https://github.com/Healthapp-org/G5T5-CI-N-Stage.git']]])
            }
          }
          stage('2-uchenna'){
            steps{
              echo 'ps -ef'
              echo 'systemctl status Jenkins'
            }
          }
          stage('3-Ozoemena'){
            steps{
              sh 'ps -ef'
              sh 'systemctl status Jenkins'
            }
          }
        }
      }
