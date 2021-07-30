pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'echo "Built Success!"; exit 0'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		sh 'php --version'
                sh 'echo "Test Success!"; exit 0'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh 'echo "Deploy Success!"; exit 0'
            }
        }
    }
}
