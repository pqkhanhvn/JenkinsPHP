pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		pwd    
		sh scripts/build.sh
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
		/* sh 'php --version' */
                sh scripts/test.sh
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh scripts/deploy.sh
            }
        }
    }
}
