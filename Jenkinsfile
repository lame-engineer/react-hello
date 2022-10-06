pipeline {
  agent any
  tools {nodejs "nodejs"}
  stages {
    stage('Build') {
      steps {
        git 'https://github.com/lame-engineer/react-hello.git'
      }
    }
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }
    stage('Deploy') {
      steps {
        sh 'npm run build'
      }
    }    
  post {
    always {
      slackSend message: "Build deployed successfully - ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
    }
}
      }}
