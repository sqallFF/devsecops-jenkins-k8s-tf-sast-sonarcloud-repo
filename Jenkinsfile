pipeline {
  agent any
  tools { 
        maven 'Maven 3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jlewisbuggywebapp -Dsonar.organization=jlewisBuggyWebAPP -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e46de2b15860c4dc7f196ce79f96b076a561fdca'
			}
        } 
  }
}
