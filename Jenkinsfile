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
    					    	bat "docker build -t maxwellforever/testing:12 ."
    				  		bat "docker push maxwellforever/testing:12"   					    
    					}
				}
    }
}
