pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=udaybuggywebapp -Dsonar.organization=udaybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=51dcfb1090323c27cce92fa2ed39b19a4f6dc224'
			}
        } 
  }
}
