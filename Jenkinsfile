pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git branch: 'main', url: 'https://github.com/MaxwellMendes90/Api.DotNetCore.git'
            }
        }
        stage('Build') {
    					steps {
    					    	bat "docker build -t maxwellforever/testing:$(BUILD_NUMBER) ."
    				  		bat "docker push maxwellforever/testing:$(BUILD_NUMBER)"   					    
    					}
				}
    }
}
