
pipeline {
	agent {
		label 'master'
		}
	stages {
		stage('Greeting') {
			steps {
				sh 'echo "notification time"'
				}
			}
		}
	post {
		success {
			emailext(
				subject: "${env.JOB_NAME} [${env.BUILD_NUMBER}] Ran!",
				body: """
				'${env.JOB_NAME} [${env.BUILD_NUMBER}]' Ran!" : Check console output at ${env.JOB_NAME} [${env.BUILD_NUMBER}]/a> """, to: "himanshu.shukla08@gmail.com" ) } } }



 


