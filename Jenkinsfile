pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/Devops-trainer1987/cts2021.git'
         }
      }
      stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/Windows/System32/config/systemprofile/AppData/Local/Jenkins/.jenkins/jobs/cts_pipeline01/workspace/target/cts-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
