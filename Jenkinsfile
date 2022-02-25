pipeline {
    steps {
    sh "apt-get update && apt-get install ssh -y"
    // rest of your steps here...
}
    agent { docker { image 'maven:3-openjdk-8-slim' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
     stage ('Deploy-To-Tomcat') {
            steps {
           sshagent(['tomcat']) {
                sh 'scp -o StrictHostKeyChecking=no target/*.war vagrant@tomcat:/home/vagrant/apache-tomcat-9.0.58/webapps/webapp.war'
              }      
           }
       }  
    }
}
