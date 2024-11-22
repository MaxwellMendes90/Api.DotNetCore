pipeline {
    agent {
	    label 'WindowsJenkinsAgent'
    }

    stages {
	    stage('Checkout')
	    {
        	steps
	    	{
				echo "I	m here" 

				cleanWs()
				
				checkout scm
  		    }
	    }
    }
}
