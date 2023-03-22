// node {  
//     stage('Build') { 
//         echo "BUILD"
//         sh "pwd"
//         sh "ls"
//     }
//     stage('Test') { 
//         echo "TEST"
//     }
//     stage('Deploy') { 
//         echo "Deploy"
//     }
// }

// DECLARATIVE
pipeline {
	agent { docker  {} }
	// agent any
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