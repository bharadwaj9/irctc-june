pipeline {
    agent { label 'label2' }
	
	tools { 
	    jdk 'javalinuxslave'
        maven 'maven2' 

		}

    stages {
        stage('Build') {
            steps {
               sh '''mvn clean install'''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}