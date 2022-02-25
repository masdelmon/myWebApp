pipeline {
    agent { docker { image 'maven:3-openjdk-8-slim' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
     stage ('Deploy-To-Tomcat') {
            steps {
           sh "sudo apt-get install ssh -y"
           sshagent(credentials: ['292d2a70-634c-4169-a1a4-6d42b3c31872']) {
                sh 'scp -o StrictHostKeyChecking=no target/*.war vagrant@tomcat:/home/vagrant/apache-tomcat-9.0.58/webapps/webapp.war'
              }      
           }
       }  
    }
}
