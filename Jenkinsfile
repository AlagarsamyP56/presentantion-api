pipeline {
    agent any
    stages {
        stage('Build Application') {
            steps {
                script {  
                        bat 'mvn clean install'   
                }
            }
        }
        stage('Deploy CloudHubs') {
            steps {
                script {
                        bat "mvn clean deploy -DmuleDeploy "
                }
            }
        }
    }
}