pipeline {
	agent any
		stages {
			stage('One') {
				steps {
					sh '''
						echo "Step One from third commit "
					'''
				}
			}


			stage('Two') {
				steps {
					sh '''
						echo "Step Two from third commit"
					'''
				}
			} 

			stage('Three') {
				steps {
					sh '''
						echo "Step Three from third commit"
					'''
				}
			}
		}
}

