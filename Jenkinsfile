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
    stage('Test') {
      steps {
        sh 'npm run deploy'
      }    
    }    
}}
