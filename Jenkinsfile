pipeline{
	agent any
	
	stages{
		stage("Build"){
			steps{
				sh "mvn -vesrion"
				sh "mvn clean install"
			}
		}
	}
	
	post{
		always{
			cleanWs()
		}
	}
}