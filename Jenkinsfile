// DECLARATIVE

pipeline {
	// agent { docker  {} }
	agent any
	stages {
		stage('Build') {
			steps {
				sh "docker --version"
				echo "Build"
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