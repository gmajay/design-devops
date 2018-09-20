node {
    stage 'Clone the project'
    git 'https://github.com/eugenp/tutorials.git'
   
    dir('pipeline-test') {
        stage("Compilation and Analysis") {
            parallel 'Compilation': {
                sh "./mvnw clean install"
            }
	  }
	}
}	

