pipeline
{
	agent any
	stages{
		stage('Build Application'){
			steps{
				bat 'mvn clean install'
			}
		}
		stage('MUnit Test Application'){
			steps{
				bat 'mvn test'
			}
		}
		stage('Deploy Application to CloudHub'){
			steps{
				bat 'mvn package deploy -DmuleDeploy'
			}
		}	
	}
}