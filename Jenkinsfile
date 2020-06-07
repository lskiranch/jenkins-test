pipeline {
  agent any
  stages {
    stage('Build/Linux') {
      parallel {
        stage('Build/Linux') {
          steps {
            echo 'This is Building stage'
          }
        }

        stage('Build/Windows') {
          steps {
            echo 'It\'s windows build'
          }
        }

        stage('Build/android') {
          steps {
            echo 'It\'s Android'
          }
        }

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