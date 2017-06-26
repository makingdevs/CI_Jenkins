#!/usr/bin/env groovy

pipeline {

  agent {
    node {
      def imageTag = "${project}/${appName}:${env.BRANCH_NAME}.${env.BUILD_NUMBER}"
      def namespace = getNamespace(env.BRANCH_NAME)
      def environment = environmentFromBranchName(env.BRANCH_NAME)

      echo "Deploy config with environment: ${environment} namespace: ${namespace}"

    }
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
  }
}
