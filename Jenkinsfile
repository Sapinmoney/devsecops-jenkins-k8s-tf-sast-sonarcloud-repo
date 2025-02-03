pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mybuggywebapp -Dsonar.organization=mybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=4a572706648dfd4ad614b43188fc01ee38506ad6'
			}
        } 
  }
}
