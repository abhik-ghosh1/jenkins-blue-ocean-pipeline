pipeline{
    agent any
    stage{
        stages('Clean'){
        	steps{
        	    bat label: '', returnStdout: true, script: 'mvn clean'
        	}
        }

    }

}
