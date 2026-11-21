pipeline {
  agent any
  tools { 
        maven 'maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=meekbuggyweb -Dsonar.organization=meekbuggyweb -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1b9867c794cbdf2dfc31536bfcbb0d1f3773f029'
			}
        } 
  }
}
