pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            	ws("/home/abhik/jenkins_ws") {
  					echo "awesome commands here instead of echo"
				}
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
