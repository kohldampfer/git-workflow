pipeline {

	agent any;

	stages {

		stage('Building') {
			steps {
				sh 'touch a.xyz'
				sh 'tar -czvf package.tar.gz *.xyz'
			}
		}

		stage('Archiving package') {
			steps {
				archiveArtifacts "package.tar.gz"
			}
		}

	}

}
