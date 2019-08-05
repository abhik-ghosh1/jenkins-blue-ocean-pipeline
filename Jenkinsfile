pipeline {
    agent any
    stages {
    	ws("/home/abhik/jenkins_ws") {
  		echo "awesome commands here instead of echo"
		}
        stage('build') {
            steps {
                sh 'mvn clean compile package --DskipTests'
            }
        }
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                sh 'mvn install -DskipTests'
            }
        }
    }
}
