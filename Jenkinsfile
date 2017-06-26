#!/usr/bin/env groovy

pipeline {

  agent any

  stages {
    stage('Build') {
      steps {
        echo "Deploy config with environment: ${env.BRANCH_NAME} namespace: ${getNamespace(env.BRANCH_NAME)}"
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
