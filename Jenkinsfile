pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				tool name: 'maven 3.3.3', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'maven 3.3.3', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'maven 3.3.3', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
