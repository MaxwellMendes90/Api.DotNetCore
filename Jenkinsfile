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
    					    	bat "dotnet restore Api.DotNetCore/Api.DotNetCore.csproj"
    				  		bat "dotnet build Api.DotNetCore/Api.DotNetCore.csproj -c Release -o /app/build"
	    			   	    bat "dotnet publish Api.DotNetCore/Api.DotNetCore.csproj -c Release -o /app/publish"
    					    
    					}
				}
    }
}
