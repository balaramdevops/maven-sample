pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'mvn clean install' 
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'cd ansible;ansible-playbook -i hosts middleware.yaml --extra-vars "WORKSPACE=${WORKSPACE}"'
            }
        }
    }
}
