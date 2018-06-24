pipeline {
	agent any

	stages {
		stage('Compile Stage') {
			steps {
					sh 'gradle clean'
			}
		}

		stage('Build Stage') {
			steps {
					sh 'gradle build'
			}
        }
	}
}
