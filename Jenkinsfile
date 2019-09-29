pipeline {
	agent {
		label 'windows'
	}
    stages {
        stage('Build') {
            steps {
				checkout scm
				bat 'npm install'
                echo 'Building..'
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
