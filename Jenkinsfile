pipeline{
	agent any
	
	tools{
		mvn "3.6.0"
	}
	
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