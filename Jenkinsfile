// DECLARATIVE

pipeline {
	agent { docker }
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