#!/usr/bin/env groovy

pipeline {

  echo "${it}"
  echo "${params.properties}"

  tools {
    jdk "jdk7"
  }

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
