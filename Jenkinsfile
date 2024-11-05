pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=exixo_org -Dsonar.organization=exixo_org -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=35a581ee8179546263aa3963765bb6ec32deb7d1'
			}
        } 
  }
}
