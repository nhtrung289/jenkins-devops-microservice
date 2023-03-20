// DECLARATIVE

pipeline {
	// agent { docker  {} }
	agent any
	environment {
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	stages {
		stage('Checkout') {
			steps {
				sh "docker version"
				sh "mvn --version"
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"
			}
		}

		stage('Compile') {
			steps {
				echo "mvn clean compile"
				// sh "mvn clean compile"
			}
		}

		stage('Test') {
			steps {
				echo "mvn test"
				// sh "mvn test"
			}
		}

		stage('Integration Test') {
			steps {
				echo "mvn failsafe:integration-test failsafe:verify"
				// sh "mvn failsafe:integration-test failsafe:verify"
			}
		}
	}
}