#!/usr/bin/env groovy

pipeline {

  println "${it}"
  println "${params.properties}"

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
