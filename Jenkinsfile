pipeline {
	agent any
	
    stages {
		stage('Build') {
			steps {
				bat "mvn clean install -Dmaven.test.skip=true"
			}
		}
		
		stage('Test') {
			steps {
				bat "mvn test"
			}
		}
	}
}