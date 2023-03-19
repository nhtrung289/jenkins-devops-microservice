// DECLARATIVE

pipeline {
	// agent { docker  {} }
	agent any
	stages {
		stage('Build') {
			steps {
				// sh "docker --version"
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Intergration Test') {
			steps {
				echo "Intergration Test"
			}
		}
	}
}