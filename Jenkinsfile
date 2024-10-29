pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=conorbuggywebapp3 -Dsonar.organization=conorbuggywebapp3 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=528d941b0416fd62297aa3c7f393158f6404b933'
			}
        } 
  }
}
