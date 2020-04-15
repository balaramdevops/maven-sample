pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the code'
                sh 'mvn clean install' 
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the app'
                sh 'cd ansible;ansible-playbook -i hosts middleware.yaml --extra-vars "WORKSPACE=${WORKSPACE}"'
            }
        }
    }
}
