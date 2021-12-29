pipeline{
	agent any
	stages{
		stage('SCM Checkout') {
			steps {
            echo "Fetch the code from BitBucket"
            sh 'sleep 3'
        }
			}
		
		stage('Maven Build'){

			steps{

				echo 'Maven Build  is in Progress'
                echo 'Artifacts are Archieved'
                sh 'sleep 3'
			}

		}
		
		stage('Dev Deployment') {

			steps{

				echo 'Deploying to Dev  Server'
                sh 'sleep 3'
				}
		}
        
		stage('Test Deployment') {
			steps{

				echo 'Tesging is going on'
                sh 'sleep 3'
			}


		}

        stage('Provide Approvals') {
			steps{

				input('Test Completed ? Please provide  Approvals for Prod Release ?')
			}
		}

		stage('Release to Prod'){

			steps{

				echo 'Prod Deployments'
                sh 'sleep 3'
			}
		}
	}
}
