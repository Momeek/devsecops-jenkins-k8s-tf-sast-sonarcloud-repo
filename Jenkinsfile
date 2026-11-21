pipeline {
  agent any
  tools { 
        maven 'maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=momeek -Dsonar.organization=Momeek -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=ad5819cdbccad3035aa04709b128bc5876f16115'
			}
        } 
  }
}
