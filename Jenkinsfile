pipeline {
    
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package'
                sh 'scp /var/lib/jenkins/workspace/Pipeline_mywebApp_master/target/web-java-spring-1.0-SNAPSHOT.war vagrant@tomcat:vagrant@tomcat:/home/vagrant/apache-tomcat-9.0.58/webapps'
            }
        }  
    }
}
