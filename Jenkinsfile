pipeline {
  agent  {label "node1"}
    stages   {
      stage("stage1") {
	  steps {
	    bat "echo stage 1"
	    bat "git clone https://github.com/santoshnh1982/LTI_Project.git"    	  
	  }
	}
    }	    
      stage("stage2") {
	  steps {
        bat 'echo stage 2' 
	    bat "mvn clean install"  	  
	  }
	} 	    
    }
