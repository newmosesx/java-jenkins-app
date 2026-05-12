pipeline {
  agent any

  tools {
    jdk 'Java'
    maven 'Maven'
  }

  stages {
    stage('Build application') {
      steps {
        sh 'echo "======== Building Java Application ========"'
        sh 'java -version'
        sh 'mvn -v'
        sh 'mvn clean package -B -DskipTests'
        sh 'echo "======== Build completed ========"'
      }
    }
  }
}
