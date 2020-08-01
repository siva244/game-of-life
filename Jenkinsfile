pipeline {
   agent any 
    stages {

    stage("scm"){
        steps{
        git 'https://github.com/siva244/spring-petclinic.git'   
    }
}
      stage("build"){
        steps{
        sh 'mvn package'  
    }
}
}
}
