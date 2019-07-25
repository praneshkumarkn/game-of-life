pipeline {
    agent any
     tools {
        maven 'maven'
        jdk 'java'
    }
    stages { 
    stage ('init') {
        steps {
            echo "PATH = ${PATH}"
            echo "M2_HOME = ${M2_HOME}"
            sh 'mvn clean compile'
    }
    }
    stage ('Build') {
        steps {

            sh 'mvn test'
    }
    }
    
    }
} 
