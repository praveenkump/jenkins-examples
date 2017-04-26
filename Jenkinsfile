node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/praveenkump/jenkins-examples'
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.           
      // mvnHome = tool 'M3'
	   bat(/"/usr/lib/jvm/java-1.7.0-openjdk-amd64","./mvnw install"/)
	    
	  archiveArtifacts artifacts: "**/target/*.*"
   }
   
 }