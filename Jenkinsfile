pipeline {
    agent any

    stages {        
        stage('Source code checkout'){
            steps {                
                git credentialsId: 'Github', url: 'https://github.com/vinomax/NewProject.git'
            }
        }
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
