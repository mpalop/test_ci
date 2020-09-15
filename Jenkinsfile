pipeline {
  agent any
  stages {
    stage ("Tests") {
      when {
        changeRequest()
      }
      steps {
        echo "testing... $BRANCH_NAME"
        echo "change ID $CHANGE_ID"
        echo "GIT_COMMIT $GIT_COMMIT"
        echo "will simulate a failure"
        exit -1 
      }
    }
  }
}
