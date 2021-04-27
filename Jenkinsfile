pipeline {
 agent any
  stages {
      stage('Compile') {
         steps {
            bat 'mvn compile'
         }
      }
      stage('Test') {
         steps {
            bat 'mvn test'
         }
      }
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
