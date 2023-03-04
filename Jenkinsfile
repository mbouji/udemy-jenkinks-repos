pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp2023 -Dsonar.organization=asgbuggywebapp2023 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=4e93a2f37d0d1386972dbcbad929767ec4fe91ef'
			}
        } 
  }
}
