pipeline {
    /*agent any*/
    agent { 
	    docker { image 'php:latest' 
		   } 
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'pwd'		
	        /*sh 'maven build' */
		/*sh 'ant build' */
		/*sh 'gradle build'    */
		sh 'sh scripts/build.sh'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'		    
		/* sh 'php --version' */
                sh 'sh scripts/test.sh'
		/*sh 'unittest'*/    
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
		/* sh 'ansible deploy' */
		/* sh 'chef deploy' */    
		sh 'sh scripts/deploy.sh'
/*		sh 'exit 1'    */
            }
        }
    }
}
