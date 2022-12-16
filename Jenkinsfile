pipeline {
	agent any

	stages {
		stage('Build') {
			steps {
				sh 'docker-compose build'
			}
		}

		stage('Test') {
			steps {
				sh 'docker-compose run --rm app sh -c "python3 manage.py test"'
			}
		}

		stage('Deploy') {
			steps {
				sh 'docker-compose up -d'
			}
		}
	}
}		
