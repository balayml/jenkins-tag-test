pipeline {
    agent {
        label 'Mac_Mini'
          }
    stages {
        stage('Build') {
            steps {
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Deploy') {
            when { tag "qa-*" }
            steps {
                echo 'Deploying only because this commit is tagged...'
                
            }
        }
    }
}
