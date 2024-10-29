pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=conorbuggywebapp -Dsonar.organization=conorbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=77066bb85634a84ef70da063b71a8d0119cc90fd'
			}
        } 
  }
}
