pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=muni-bugapp -Dsonar.organization=muni-bugapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b3d244186c7082bfe573f2c7aa345466833b084e'
			}
        } 
  }
}
