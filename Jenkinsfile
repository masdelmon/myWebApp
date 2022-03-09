  pipeline {
    
    agent any
    stages {
        stage('build') {
            steps {
                sh 'sudo su jenkins && mvn clean package'
            }
        }  
      }
}
