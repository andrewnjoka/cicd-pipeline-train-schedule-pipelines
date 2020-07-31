pipeline {
	agent any
	stages {
		stage ('build') {
			steps {
				echo 'running build automation now'
				sh './gradlew build --no-daemon'
				archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
