#!groovy

node {
	   
	stage('Checkout'){

          checkout scm
       }

       stage('BuildArtifact'){

         // sh 'mvn install'
	       
	       bat 'mvn clean deploy'
       }
	   
      stage('Sonar') {
                    //add stage sonar
                   bat 'mvn sonar:sonar'
                }
	
       
}
