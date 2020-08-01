pipeline {
   agent any 
    stages {

    stage("scm"){
        steps{
        git 'https://github.com/siva244/game-of-life.git'   
    }
}
      stage("build"){
        steps{
        sh 'mvn clean package'  
    }
}
}
}
