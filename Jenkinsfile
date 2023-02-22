pipeline {
	agent any
	stages {
		stage('Clone stage') {
			steps {
				git 'https://github.com/binhquangthuy/Angular-Full-Course---Complete-Zero-to-Hero-Angular-full-Tutorial.git'
			}
		}
		stage('build stage') {
			steps {
				sh 'docker build -t binhquangthuy/docker-test'
				sh 'docker push binhquangthuy/docker-test'
			}
		}
	}
}
