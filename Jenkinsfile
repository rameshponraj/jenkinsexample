pipeline {
    agent any
        stages {
            stage('Compile stage') {
                steps {
                    maven(maven : 'Maven_4.0.0'){
                        bat "mvn clean compile"
                    }
                }
            }
        stage('testing stage') {
            steps {
                maven(maven : 'Maven_4.0.0'){
                    bat "mvn test"
                }
            }
        }
        stage('deployment stage') {
            steps {
                maven(maven : 'Maven_4.0.0'){
                    bat "mvn deploy"
                    }
                }
            }
        }
    }