pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script {
						env.EXECUTE=true
					}
	
				}
			}


			stage('Second') {
				when {${EXECUTE}=true
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

