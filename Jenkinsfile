node {
    stage 'Clone the project'
    git  'https://github.com/gmajay/design-devops.git'
   
    dir('pipeline-test') {
        stage("Compilation and Analysis") {
            parallel 'Compilation': {
                sh "./mvnw clean install"
            }
	  }
	}
}	

