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
				withDockerRegistry(credentialsId: 'docker-hub-id', url: 'https://index.docker.io/v1/') {
    					sh 'docker build -t binhquangthuy/docker-test:v1 .'
					sh 'docker push binhquangthuy/docker-test:v1'
				}
				
			}
		}
	}
}
