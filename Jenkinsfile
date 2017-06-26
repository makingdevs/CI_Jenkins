#!/usr/bin/env groovy

pipeline {

  agent any

  parameters {
    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
  }

  tools {
    maven 'apache-maven-3.0.1'
  }

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
    stage('Example') {
      steps {
        echo "Hello ${params.PERSON}"
      }
    }
    stage('Example2') {
      steps {
        sh 'mvn --version'
      }
    }
  }
}
