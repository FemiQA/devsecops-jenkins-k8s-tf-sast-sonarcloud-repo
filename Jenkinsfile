pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_9'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=qabuggywebapp -Dsonar.organization=qabuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c04c2993c61c01642cdcbd6cf105874f625cb6e8'
			}
        } 
  }
}
