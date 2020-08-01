	pipeline{
	agent any
	stages {
		stage('scm'){
			steps{
			git 'https://github.com/wakaleo/game-of-life.git'
		}
		}
		
		 stage('build'){
			 steps{
			sh label: '', script: 'mvn package'
		}
		 }
		 stage('postbuild'){
			 steps{
			junit 'gameoflife-web/target/surefire-reports/*.xml'
			archiveArtifacts artifacts: 'gameoflife-web/target/*.war', followSymlinks: false
		}
		 }
	}
	}
