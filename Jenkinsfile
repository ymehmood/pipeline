pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I am in Build'
        sh 'echo "AOA !"'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Starting Test'
          }
        }
        stage('Unit Test') {
          steps {
            echo 'In Unit Test'
          }
        }
        stage('Integration Test') {
          steps {
            echo 'In Integration Test'
          }
        }
      }
    }
    stage('Install/Stage') {
      steps {
        echo 'In stage'
      }
    }
    stage('L0 - Deploy') {
      steps {
        echo 'Deploying L0'
      }
    }
    stage('L1 - Deploy') {
      steps {
        echo 'Deploying L2'
      }
    }
  }
}