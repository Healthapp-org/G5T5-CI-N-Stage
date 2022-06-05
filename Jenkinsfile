pipeline{
      	agent any 
      	tools{}
      	stages{
      		stage('1-git checkout'){
      			steps{
      			  git branch: checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'f7c765a1-e95f-44ad-9f53-7b9fc6ad20ec', url: 'https://github.com/Healthapp-org/G5T5-CI-N-Stage.git']]])'
      			}
      		}
      		stage('2-systemanalysis'){
      			steps{
      				sh ' lscpu '
      			}
      		}
      		stage('3-storage'){
      			steps{
      				sh 'df -h'
      				sh 'free -g'
      			}
      		}
                stage('4-Uchenna'){
                  steps{
                    echo 'ps -ef'
                    echo 'sudo systemctl status Jenkins'
                  }
      	}
      }
