pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                dir("NikhilJain_RestfulAndSoapWS") {
		bat "mvn clean"
	}
            }
        }
        stage('Compile') {
            steps {
	dir("NikhilJain_RestfulAndSoapWS") {
		bat "mvn compile"
	}
            }
        }
        stage('Test') {
            steps {
	dir("NikhilJain_RestfulAndSoapWS") {
		bat "mvn test"
	}
            }
        }
        stage('Result') {
            steps {
                echo "Result"
            }
        }
    }
}