pipeline {

    agent any
    tools {
        maven 'apache-maven-3.6.3'
    }
    stages {
        stage('Compile stage') {
            steps {
                sh "mvn clean compile"
        }
    }

         stage('testing stage') {
             steps {
                sh "mvn test"
        }
    }

          stage('install stage') {
              steps {
                sh "mvn install"
        }
    }

  }

}