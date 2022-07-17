pipeline {
    agent { docker { image 'maven:3.8.4-openjdk-11-slim' } }
    stages {
        stage('compile') {
            steps {
              withMaven(maven : apache-maven-3.8.6 )
                sh 'mvn clean compile'
            }
        }
    }
}