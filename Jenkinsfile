  pipeline {
    
    agent any
    stages {
        stage('build') {
            steps {
                sh 'clean package -Dmaven.test.skip=true com.hello2morrow:sonargraph-maven-plugin:12.0.5:create-report -Dsonargraph.sonargraphBuildVersion=8.7.0 -Dsonargraph.reportFormat=xml -Dsonargraph.prepareForSonarQube=true  -Dsonargraph.installationDirectory=/home/vagrant/SonargraphBuild-12.0.5.717_2022-02-25  -Dsonargraph.licenseFile=/home/vagrant/Sonargraph.license  -Dsonar.sonargraph.integration:report.path=/var/lib/jenkins/workspace/demo_master/target/sonargraph/sonargraph-sonarqube-report.xml'
            }
        }  
      }
}
