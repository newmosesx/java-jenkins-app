pipeline{

  agent any
  
  tools {
    // '<name of tool>' given in the manage jenkins > Tools > Maven Installation
    maven 'Maven'
  }

  stages{

      stage('building the application'){
        steps{
            sh 'echo "========Building Java Application============"'
            sh 'mvn -v'
            sh 'mvn clean package -B -DskipTests'
            sh 'echo "======Building Java Application completed====="'
          
        }
      }
 
  }
}
