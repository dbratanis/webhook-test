#!/usr/bin/env groovy

pipeline {
    agent any
  stages {
    stage('Build') {
     when {
        not {
            branch '*WIP*'
        }
        beforeAgent true
      }
      parallel {
        stage("Build 1") {
          steps {
            echo 'Build 1'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
        stage("Build 2") {
          steps {
            echo 'Build 2'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
        stage("Build 3") {

          steps {
            echo 'Build 3'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
      }
    }
    stage('Test') {
     when {
        not {
            branch '*WIP*'
        }
        beforeAgent true
      }
      parallel {
        stage("Test 1") {
          steps {
            echo '1'
            sh 'echo ${BRANCH_NAME}'
            echo '2'
            sh 'echo ${BRANCH}'
            echo '3'
            sh 'echo ${GIT_BRANCH}'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
        stage("Test 2") {
          steps {
            echo 'Test 2'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
        stage("Test 3") {
          steps {
            echo 'Test 3'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
        stage("Test 4") {
          steps {
            echo 'Test 4'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
        stage("Test 5") {
          steps {
            echo 'Test 5'
          }
          post {
            success {
              echo "Build succesfull"
            }
            failure {
              echo "Build failure"
            }
          }
        }
      }
    }
    stage('Web 1') {
     when {
        not {
            branch '*WIP*'
        }
        beforeAgent true
      }
      steps {
        echo 'Web 1'
      }
      post {
        success {
          echo "App succesfully deployed to Elastic Beanstalk Env"
        }
        failure {
          echo "App deployment failed to Elastic Beanstalk Env"
        }
      }
    }
  }
}
