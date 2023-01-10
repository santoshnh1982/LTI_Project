pipeline {
  agent any
    stages {
      stage("Checkout") {
        parallel{
          stage("parallel1"){
            steps{
              bat "echo parallel1"
            }
          }
          stage("parallel2"){
            steps {
              bat "echo parallel2"
            }
          }
        }
      }
      stage("build only") {
        steps {      
          bat 'mvn clean install'        
        }
      }
         
}
