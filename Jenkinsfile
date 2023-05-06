#!/usr/bin/env groovy

pipeline {
    agent any
    tools{
        maven 'maven-3.9'
    }
    stages {
        stage('build') {
            steps {
                script {
                    echo "building the application..."
                    sh "mvn package"
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
                    sh 'java -jar SearchMicroservices-0.0.1-SNAPSHOT.jar'

                }
            }
        }
    }
}
