pipeline {
    agent { docker { image 'maven:3-openjdk-8-slim' } }
    
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }  
    }
}
