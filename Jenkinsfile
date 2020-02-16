pipeline
{
	agent any
	
		stages 
		{
				 stage('clone') {
					steps {
						echo 'cloning..'
					}
			}
				stage('Test') {
					steps {
						echo 'Testing..'
				}
				
				stage('Get approval'){
    					input "Deploy to qa?"
					}
				node {
					    stage('deploy to qa'){
						echo "deploying"
					    }
					}
			
				stage('Build') {
				steps {
					echo 'Building....'
				}
			}
			
		}
	
}
