pipeline {
    
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('deploy') {
        withCredentials([sshUserPrivateKey(credentialsId: "	292d2a70-634c-4169-a1a4-6d42b3c31872", keyFileVariable: 'my_private_key_file')]) {
            sh "scp -i ${my_private_key_file} -v vagrant@tomcat:/var/lib/jenkins/workspace/Pipeline_mywebApp_master/target/web-java-spring-1.0-SNAPSHOT.war /home/vagrant/apache-tomcat-9.0.58/webapps"
        }
    }
    }
}
