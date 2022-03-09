  pipeline {
    
    agent any
    stages {
        stage('build') {
            steps {
                sh 'clean package -Dmaven.test.skip=true com.hello2morrow:sonargraph-maven-plugin:12.0.5:create-report -Dsonargraph.sonargraphBuildVersion=8.7.0 -Dsonargraph.reportFormat=xml -Dsonargraph.prepareForSonarQube=true  -Dsonargraph.installationDirectory=E:\Download\products\SonargraphBuild\dist\release\SonargraphBuild  -Dsonargraph.licenseFile=E:\Download\Sonargraph.license  -Dsonar.sonargraph.integration:report.path=E:/Download/Sonargraph9_WalkThroughTutorial_Project/crm-domain-example/target.maven/sonargraph/sonargraph-sonarqube-report.xml'clean package -Dmaven.test.skip=true com.hello2morrow:sonargraph-maven-plugin:12.0.5:create-report -Dsonargraph.sonargraphBuildVersion=8.7.0 -Dsonargraph.reportFormat=xml -Dsonargraph.prepareForSonarQube=true  -Dsonargraph.installationDirectory=E:\Download\products\SonargraphBuild\dist\release\SonargraphBuild  -Dsonargraph.licenseFile=E:\Download\Sonargraph.license  -Dsonar.sonargraph.integration:report.path=/var/lib/jenkins/workspace/demo_master/target/sonargraph/sonargraph-sonarqube-report.xml
            }
        }  
      }
}
