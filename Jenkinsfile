pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=classkey -Dsonar.organization=classkey -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=14a41e6b2d17f65e4473c440f5e1c9f7d9583be5'
			}
        } 
  }
}
