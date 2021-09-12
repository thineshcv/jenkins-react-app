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
    
}
