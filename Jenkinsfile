pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=udaybuggywebapp -Dsonar.organization=udaysairajujempana -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=460a499e8d80d82171867e00ff438d6b13f420c2'
			}
        } 
  }
}
