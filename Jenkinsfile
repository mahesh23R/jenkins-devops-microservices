pipeline {
	agent any
	//agent { docker { image 'maven:latest'} }
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				echo "Build"
				echo "PATH - $PATH"
				echo "BUIDL_NUMBER - $env.BUIDL_NUMBER"
				echo "BUIDL_ID - $env.BUIDL_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUID_TAG - $env.BUID_TAG"
				echo "BUID_URL - $env.BUID_URL"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} 
	
	post {
		always {
			echo 'Iam awesome I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when u fail'
		}
	}
}
