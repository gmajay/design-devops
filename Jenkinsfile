pipeline {
	agent any    
    stages{
	checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: 
	[[url: 'https://github.com/gmajay/design-devops.git']]])
       	} 
    }



