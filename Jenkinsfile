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
    					    bat "\"${tool 'MSBuild'}\" Api.DotNetCore.sln  /t:restore  /p:outdir=Publish /p:deployonbuild=true /p:Configuration=Debug /p:Platform=\"Any CPU\" "
    					    //powershell 'MsBuild MVC.sln   /t:restore /t:build /p:Configuration=Debug /p:Platform="Any CPU"'
    					    
    					}
				}
    }
}