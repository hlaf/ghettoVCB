#!groovy

@Library('emt-pipeline-lib@latest') _

node('docker-slave') {
  
  try {

    stage('commit.checkout') {
    }

    stage('commit.tests.unit') {
    }

    stage('commit.tests.integration') {
    }

    stage('release') {
    }

  } catch(e) {
    currentBuild.result = 'FAILED'
    notifyBuild(currentBuild.result, 'hlaf@emtegrity.com')
    throw e
  }
}
