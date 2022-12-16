#def name = "karlo"

pipeline {
	agent any

	stages {
		stage("verify tooling") {
			steps {
				sh '''
					docker version
					docker info
					docker compose version
					vurl --version
					jq --version
				'''
			}
		}
	}
}
#		stage('Test') {
#			steps {
#				sh 'docker-compose run --rm app sh -c "python3 manage.py test"'
#			}
#		}
#
#		stage('Deploy') {
#			steps {
#				sh 'docker-compose up -d'
#			}
#		}
#	}
#}		
