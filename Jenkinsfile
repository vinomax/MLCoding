pipeline {
    agent any

    stages {        
        stage('Build') {
            steps {
                bat '''
                cd WebApp
                mvn clean install
                '''
            }
        }
    }
}
