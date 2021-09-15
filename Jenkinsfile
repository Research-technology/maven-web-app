node {
    def mavenHome = tool name: 'maven3.8.2'
  stage('1-Clone') {
   git credentialsId: 'github credential ', url: 'https://github.com/Research-technology/maven-web-app.git'
  }
stage('2-mavenBuild') {
     sh "${mavenHome}/bin/mvn clean package"
}
 /*
    stage('3-CodeQuality') {
      sh "${mavenHome}/bin/mvn sonar:sonar"
  }
stage('4. Approval') 
{
echo "Approved. Ready for deployment"
}
stage('5. DeployTomcat') 
{
deploy adapters: [tomcat9(credentialsId: 'tomcat1', path: '', url: 'http://3.131.100.13:8080/')], contextPath: null, war: 'target/*war'
}
stage('6. Notification') 
{
emailext body: '''hello Everyone,
Build from Ebay pipeline project. 
Elizabeth Adewole ''', recipientProviders: [developers()], subject: 'Build  status ', to: 'Developers'
}
*/
}
