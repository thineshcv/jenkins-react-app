pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('source') {
            steps {
                git 'git@github.com:thineshcv/jenkins.git'
            }
        }
	stage('test') {
		steps {
			sh 'yarn test'
		}
	}
	stage('Docker Image') {
		steps {
			sh 'docker image build -t react-app:0.1 ."
		}
   	 }

    }
}
