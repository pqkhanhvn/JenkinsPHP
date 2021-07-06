pipeline {
    agent { docker { image 'php' } }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
                sh 'pwd'
            }
        }    
        stage('Test') {
            steps {
                sh 'echo "Fail!"; exit 1'
            }        
    }    
}
