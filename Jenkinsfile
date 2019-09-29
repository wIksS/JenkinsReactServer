pipeline {
	agent any
    stages {
        stage('Build') {
            steps {
			    echo 'Building..'
				checkout scm
				bat 'npm install'
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
				bat 'npm run build'
            }
        }
    }
}
