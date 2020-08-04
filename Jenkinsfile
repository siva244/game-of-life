pipeline {
  agent any                     
  triggers { 
     upstream(upstreamProjects: "dummy", threshold: hudson.model.Result.SUCCESS)
}
     
   stages{
     stage('clone and compile'){
      steps {
        git branch: 'declarative', url: 'https://github.com/siva244/game-of-life.git' 
}
}
       stage('build'){
            steps {		
         sh 'mvn clean package' 
		 input 'continue to next step?'
		 archiveArtifacts 'pipeline-gol/*.war'
 
}
}
}
}
