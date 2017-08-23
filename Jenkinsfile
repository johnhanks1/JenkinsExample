pipeline {
  agent any
  stages {
   stage('Build') {
     steps {
       awsCodeBuild projectName: 'JenkinsPipelineExample',
                   credentialsId: 'pipelineExample',  
                   credentialsType: 'jenkins',
                   region: 'us-east-1',
                   sourceControlType: 'jenkins'
     }
   }
  }
}
