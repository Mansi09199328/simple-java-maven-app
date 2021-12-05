
pipeline {
    agent { 
	 label'master'

	}
	tools{ 
	maven 'mymaven'
	jdk 'java'
	}
    stages {
 
       stage('validate') {
            steps {
                sh 'mvn validate'
            }
			stages {
 
       stage('compile') {
            steps {
                sh 'mvn compile'
            }
			stages {
 
       stage('test') {
            steps {
                sh 'mvn -test'
            }
			stages {
 
       stage('package') {
            steps {
                sh 'mvn package'
            }
			           }
        }
    }
}
