pipeline {
  stages {
    stage('Build') {
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
      parallel {
        stage("Test 1") {
          steps {
            echo 'Test 1'
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
