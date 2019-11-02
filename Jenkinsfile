pipeline {
    agent any

    stages {
		stage('Checkout external proj') {
			steps {
				echo "Checking out scm..."
				git 'https://github.com/Snefff/testCI.git'
			}
		}
        stage('Build') {
            steps {
                echo 'Building..'
				bat label: '', script: 'cd maven-demo-1'
				bat label: '', script: 'mvn install'
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