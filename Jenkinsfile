pipeline {
    agent any
    environment {
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    }
    stages {
        stage("Checkout") {
            steps {
                git credentialsId: 'rcaws22', url: 'https://github.com/rcaws22/hello-world.git'
            }
        }
        stage("build"){
          steps{
              sh 'mvn clean install'
          }
      }
   }
 }
