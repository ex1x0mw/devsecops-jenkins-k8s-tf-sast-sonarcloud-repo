pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=exixo-org_chiso -Dsonar.organization=exixo_org -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=dcdf8a984329797af273b3360f42040fb631a763'
			}
        } 
  }
}
