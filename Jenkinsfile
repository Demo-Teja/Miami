#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: 'Teja',
    projectUrlStr: 'https://github.com/Demo-Teja/Miami.git'],
    pipelineTriggers([upstream('Demo-Teja'),
githubPush()])])

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
