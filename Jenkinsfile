pipeline {
    agent any
    stages {
        stage("deploy") {
            steps {
                git clone ''
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
