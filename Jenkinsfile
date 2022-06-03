pipeline {
agent any

stages {
         
           stage('Cloning our Git') {

            steps {
                git credentialsId: 'git-credentials', url: 'https://github.com/kliakos/sparkjava-war-example.git'
                //git branch: 'master', url: 'https://github.com/kliakos/sparkjava-war-example.git'
                sh 'ls'

            }

             }
		
		   stage('build') {
		   
		   steps {
		        //buildInfo = rtMaven.run pom: 'maven-example/pom.xml', goals: 'clean install'
		     sh "mvn install"
		   }
		   }
		   
		   stage('deployment') {
		   
		   steps {
        sh "cd /etc/ansible/
		   sh "ansible --version"
		   }
		   }


}



}
