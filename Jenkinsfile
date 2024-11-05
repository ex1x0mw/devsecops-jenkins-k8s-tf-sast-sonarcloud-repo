pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=exixo-org_exixo-scan -Dsonar.organization=exixo-org -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=18168ee661575b2ddbcc7b2c3363b31928e5a64d'
			}
        } 
  }
}
