pipeline {
	agent any

	stages {
		stage('Compile Stage') {
			steps {
					withGradle(gradle : 'gradle-4.5.1') {
					sh 'gradle clean'
				}
			}
		}

		stage('Build Stage') {
			steps {
					withGradle(gradle : 'gradle-4.5.1') {
					sh 'gradle build'
				}
        	}
        }

		stage('Deploy Stage') {
			steps {
					withGradle(gradle : 'gradle-4.5.1') {
					sh 'gradle bootRun'
				}
        	}
        }

	}
}
