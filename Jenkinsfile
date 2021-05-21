pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script {
						env.EXECUTE='true'
					}
	
				}
			}


			stage('Second') {
				when { environment name: 'EXECUTE', value: 'true'
				
				}
				steps {
					sh '''
						echo "Update Second Stage"
					'''	
				}
			
			} 

			stage('Third') {
				when { environment name: 'EXECUTE', value: 'false'

                                }
				steps {
					sh '''
						echo "Step three"
					'''
				}
			}
		}
}

