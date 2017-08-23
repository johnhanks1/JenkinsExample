pipeline {
  agent any
  stages {
   stage('Build') {
     steps {
       awsCodeBuild projectName: 'JenkinsPipelineExample',
                   credentialsType: 'keys',
                   awsAccessKey: AWS_ACCESS_KEY_ID,
                   awsSecretKey: AWS_SECRET_ACCESS_KEY,
                   region: 'us-east-1',
                   sourceControlType: 'jenkins'
     }
   }
  }
}
