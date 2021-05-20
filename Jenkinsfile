pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script {
						env.EXECUTE="True"
					}
	
				}
			}


			stage('Second') {
				when {${EXECUTE} equals ="True"
				}
				steps {
					sh '''
						echo "Update Second Stage"
					'''	
				}
			
			} 

			stage('Third') {
				steps {
					sh '''
						echo "Step Three from third commit"
					'''
				}
			}
		}
}

