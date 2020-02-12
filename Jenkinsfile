pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				tool name: 'jdk 1.8.211', type: 'JDK'
				tool name: 'maven 3.3.3', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'jdk 1.8.211', type: 'JDK'
				tool name: 'maven 3.3.3', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'jdk 1.8.211', type: 'JDK'
				tool name: 'maven 3.3.3', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
