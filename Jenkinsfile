pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		echo "Built Success!";
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		/* sh 'php --version' */
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
