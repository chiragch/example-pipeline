pipeline{
	agent any
	stages{
	    stage('checkout'){
	      	steps{
	      	git credentialsId: 'f1238b79-8225-4562-9035-60756ed108b0', url: 'https://github.com/chiragch/Music_Store.git'
	      	}
	    }
		stage('Build'){
			steps{
				echo 'Building..'
			}
		}
		stage('Test'){
			steps{
				echo 'Testing..'
			}
		}
		stage('Deploy'){
			steps{
				echo 'Deploying..'
			}
		}
		stage('Example'){
			steps{
				echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
			}
		}
	}
}