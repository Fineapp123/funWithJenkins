pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/Fineapp123/funWithJenkins/'
            }
        }		
		stage('Build'){
			steps{
				sh 'echo "Building app"'
			}
		}
	    stage('Test'){
			steps {
			 sh 'echo "Running Tests"' 
			}
			}
		stage('Deploy'){
			steps {
			 sh 'echo "Deploying"'  
			}
			}
    }
}
post{
	success{
		bat 'echo "Build succesful"'
	}
	failure{
		bat 'echo "Build failed"'
	}
}

