pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=conorbuggywebapp3 -Dsonar.organization=conorbuggywebapp3 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a5ff4e5d94b3576dbbb2a4740a9d3b0a336060ca'
			}
        } 
  }
}
