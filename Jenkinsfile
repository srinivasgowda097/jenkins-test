#!/usr/bin/groovy

node {
   def mvnHome
   stage('Setup') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/jglick/simple-maven-project-with-tests.git'
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.           
      mvnHome = "/apache-maven/"
      sleep 100
   }
   stage('Dev') {
      // Run the maven build
     echo "Done"
     sleep 60
      
   }
   stage('Teardown') {
      
      archive '*.*'
      sleep 4
   }
}
