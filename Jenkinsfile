pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
              //sh 'cd spring-petclinic'
              //sh 'mvnw package'
              sh 'mvn package'
              sh 'java -jar target/*.jar'
            }
        }
    }
}
