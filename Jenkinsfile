pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'               
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
            	bat 'mvn clean package deploy -DmuleDeploy'
                echo 'Deploying....'
            }
        }
    }
}