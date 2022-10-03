pipeline {
    agent any
    stages {
        stage("deploy") {
            steps {
                git clone 'https://github.com/lame-engineer/react-hello.git'
                npm start 
            }
        }
        stage("after-deploy") {
            steps {
                   echo "success!!!" 
            }
        }
    }
}
