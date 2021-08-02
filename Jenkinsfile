pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'pwd'    
		sh 'sh scripts/build.sh'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'		    
		/* sh 'php --version' */
                sh 'sh scripts/test.sh'
		sh 'maven test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		sh 'sh scripts/deploy.sh'
            }
        }
    }
}
