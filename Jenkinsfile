pipeline {
  agent any
  stages {
   stage('Build') {
     steps {
       awsCodeBuild projectName: 'project',
                   credentialsType: 'keys',
                   awsAccessKey: AWS_ACCESS_KEY_ID,
                   awsSecretKey: AWS_SECRET_ACCESS_KEY,
                   region: 'us-west-2',
                   sourceControlType: 'jenkins'
     }
   }
  }
}
