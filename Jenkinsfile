pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_6'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dbak3ybugywebapp -Dsonar.organization=dbak3ybugywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=5169cafefbe8232c4f60dbbbbaf3995de3e750fb'
			}
        } 
  }
}
