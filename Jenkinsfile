pipeline {
      agent any
      tools{
            Maven_3_5_2
      }

      stages{
            stage('ComplieandRunSonar')
            {
                  steps{
                        sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyProject -Dsonar.organization=buggyWebApp_pramod -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2da80038c47581ae151ae805a7a2e4d755077af7'
                  }
            }
      }
}