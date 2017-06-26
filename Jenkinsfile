#!/usr/bin/env groovy

pipeline {

  agent any

  tools {
    maven 'apache-maven-3.0.1'
    //jdk 'JDK7u80'
  }

  stages {
    stage('Build') {
      steps {
        echo "Deploy config with environment: ${env.BRANCH_NAME} "
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
    stage('Example2') {
      steps {
        sh 'mvn --version'
      }
    }
    stage("Clean and compile"){
      steps{
        sh './grailsw clean --plain-output --non-interactive'
        sh 'rm -fR target/test-reports'
      }
    }
  }
}
