pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh ''g++ -o a.exe helloa.cpp'
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                echo 'Starting Testing'
                sh './a.exe'
                echo 'Test Completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Starting Deploy'
                echo 'Deploy Completed'
            }
        }
    }
  post {
    failure {
      echo 'Pipeline Failed'
    }
  }
}
