pipeline {
    agent any
    
    tools {
        maven 'maven3.6'
        jdk 'jdk17'
    }
 
    stages {
           
        stage('Compile') {
            steps {
             bat 'mvn compile'
            }
        }
        stage('test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('Package') {
            steps {
               bat 'mvn package'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
