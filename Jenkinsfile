#!/usr/bin/env groovy

pipeline {
    agent none
    stages {
        stage('build') {
            steps {
                script {
                    echo "building the application..."
                    sh 'java --version'
//                     sh 'mvn package'
                }
            }
        }
        stage('test') {
            steps {
                script {
                    echo "Testing the application..."
                }
            }
        }
        stage('deploy') {
            steps {
                script {
                    echo "Deploying the application..."
//                     sh 'java -jar SearchMicroservices-0.0.1-SNAPSHOT.jar'
                }
            }
        }
    }
}
