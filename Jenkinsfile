@Library('shlib')_
pipeline {
    agent any
    tools {
        maven "Maven"   
    }   
  
    stages {
        stage('Compile-Build-Test ') {
            steps {
	    	                build 'BUILD'
                   }
              }
	  /*  stage('SonarQube Analysis'){
            steps{
               sonar()
            }
        }*/
              stage('Deployment'){
            steps{
               deploy_tomcat()
            }
        }
      }
  }
