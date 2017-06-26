#!/usr/bin/env groovy

pipeline {

  agent any

    stages {
      stage('Build') {
        steps {
          echo 'Building..'
          echo "${env.properties}"
        }
      }
      stage('Test') {
        steps {
          echo 'Testing..'
        }
      }
      stage('Deploy') {
        steps {
          echo 'Deploying....'
        }
      }
    }
}
