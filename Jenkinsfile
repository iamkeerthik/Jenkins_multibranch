node('master') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/iamkeerthik/Jenkins_multibranch.git'
	}
    stage('Continuous Build') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('continues deployment') 
	{
    sh 'cp /home/ubuntu/workspace/workspace/job1_loans/webapp/target/webapp.war  /var/lib/tomcat9/webapps/prod.war'
	}
}
