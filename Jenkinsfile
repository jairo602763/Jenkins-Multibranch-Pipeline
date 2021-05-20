pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					sh '''
						echo "Step One from third commit "
					'''
				}
			}


			stage('Second') {
				steps {
					sh '''
						echo "Step Two from third commit"
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

