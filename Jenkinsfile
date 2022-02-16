pipeline {
    agent any
    stages {
         stage('git clone') {
            steps {
                git 'https://github.com/letuanht/hello-world-java.git'
            }
        }
        stage('Create Docker image') {
            steps {
               sh 'docker build -t thetips4you/springboot:latest .'
              
            }
        }
        stage('Build') {
            steps {
               echo "Build completed"
            }
        }
    }
}
