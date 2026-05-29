pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=shssonarprojectkey -Dsonar.organization=shssonarkey -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c679d1aa715346269b6e0454f72cd669278dcb28'
			}
        } 
  }
}
