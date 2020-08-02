pipeline {
  agent any
  triggers { pollSCM('* * * * *')}
   stages{
     stage('clone and compile'){
      steps {
        git branch: 'master', url: 'https://github.com/siva244/game-of-life.git' 	  
         sh 'mvn compile' 
 
}
}
}
}
