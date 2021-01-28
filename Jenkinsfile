pipeline {

		agent any
		
	stages{

		
			stage('Checkout'){
        		steps{
					script {
						checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/omyy/DemoProject.git']]])
						
						//pom = readMavenPom file: 'pom.xml'
						echo "Check out done---> "+git --version// + pom.version
					}
        		}
        	}
			
		}
	}
