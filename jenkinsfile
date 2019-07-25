pipeline {
    agent any
    stages { 
    stage ('init') {
        steps {

            withMaven(maven: maven)
            sh 'mvn clean compile'
    }
    }
    stage ('Build') {
        steps {

            withMaven(maven: maven)
            sh 'mvn test'
    }
    }
    stage ('Deploy') {
        steps {

            withMaven(maven: maven)
            sh 'mvn deploy'
    }
    }
    }
} 
