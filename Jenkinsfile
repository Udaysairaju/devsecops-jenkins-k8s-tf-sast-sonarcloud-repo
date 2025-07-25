pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=udaybuggywebapp -Dsonar.organization=udaybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=51dcfb1090323c27cce92fa2ed39b19a4f6dc224'
			}
        } 
  }
}
