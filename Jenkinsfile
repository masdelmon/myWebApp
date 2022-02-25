pipeline {
    
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package && cp /var/lib/jenkins/workspace/Pipeline_mywebApp_master/target/web-java-spring-1.0-SNAPSHOT.war /home/vagrant'
            }
        }  
    }
}
