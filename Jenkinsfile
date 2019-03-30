pipeline {
    agent any
    stages {
        stage('CodeSync') {
            steps {
                git clone https://github.com/spring-projects/spring-petclinic.git
            }
        }
        stage('Build') {
            steps {
              cd spring-petclinic
              ./mvnw package
              java -jar target/*.jar
            }
        }
    }
}
