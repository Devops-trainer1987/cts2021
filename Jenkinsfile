pipeline {
 agent any
  stages {
      stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/Windows/System32/config/systemprofile/AppData/Local/Jenkins/.jenkins/jobs/cts_compile/workspace/target/cts-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
