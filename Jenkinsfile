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
	agent { docker  { image 'maven:3.6.3'} }
	// agent any
	stages {
		stage('Build') {
			steps {
				// sh "docker --version"
				echo $USER
                sh 'mvm --version'
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
	post {
			always {
				echo $USER
				echo 'Im awesome. I run always'
			}
			success {
				echo 'I run when you are successful'
			}
			failure {
				echo 'I run when you fail'
			}
	}
}