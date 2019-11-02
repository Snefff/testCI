pipeline {
    agent any

    stages {
		stage('Checkout external proj') {
			steps {
				"checking out scm"
				checkout scm
			}
		}
        stage('Build') {
            steps {
                echo 'Building..'
				mvn install
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