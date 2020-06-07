pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is Building stage'
      }
    }

    stage('test') {
      steps {
        echo 'This is Testing stage'
      }
    }

    stage('Approval') {
      steps {
        input 'Approve this flow'
      }
    }

    stage('Deploy') {
      steps {
        echo 'To deploy it '
      }
    }

  }
}