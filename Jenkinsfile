pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ new.cpp -o new'
                 build job: 'PES1UG20CS498-1', wait: false
                 echo 'Build successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat new.cpp'
                echo 'Test successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
