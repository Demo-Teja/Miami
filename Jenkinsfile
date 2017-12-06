#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: 'Teja',
    projectUrlStr: 'https://github.com/Demo-Teja/Miami.git'],
    pipelineTriggers([
        upstream(
     threshold: 'SUCCESS',
     upstreamProjects:'https://github.com/Demo-Teja/omaha.git'
        )
            ])
         ])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
