pipeline {
  agent any
  tools {nodejs "node"}
  stages {
    stage('Build') {
      steps {
        git 'https://github.com/lame-engineer/react-hello.git'
        sh 'npm install'
        sh 'npm start'
      }}}}
