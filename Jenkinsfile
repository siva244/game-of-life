pipeline {
  agent any
  triggers { 
     upstream(upstreamProjects: 'dummy',threshold: hydson.model.Result.SUCCESS)
     }
   stages{
     stage('clone and compile'){
      steps {
        git branch: 'declarative', url: 'https://github.com/siva244/game-of-life.git' 	  
         sh 'mvn compile' 
 
}
}
}
}
