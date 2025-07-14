pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=daavulnresearch -Dsonar.organization="Ervin Zhao" -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=663a4a7540ef90721bc050da5b34e02131decfe9'
			}
        } 
  }
}
