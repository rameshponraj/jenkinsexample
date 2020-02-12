pipeline {

    agent any
    tools {
        maven 'Maven_4.0.0'
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile"
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

          stage('deployment stage') {
              steps {
                bat "mvn deploy"
        }
    }

  }

}