pipeline{
	agent{
		docker{
			image "maven:3.6.0-jdk-13"
			label "docker"
		}
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