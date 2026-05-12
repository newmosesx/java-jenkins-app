pipeline{
  
  agent any
  
  tools {
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
