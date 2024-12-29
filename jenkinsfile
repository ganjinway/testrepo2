pipeline {
    agent { 
        node {
            label 'app'
            }
      }
    triggers {
        pollSCM '*/5 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                bat """
                cd c:\\
                echo %errorlevel%
                """
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                bat """
                cd c:\\
                dir c:\\
                """
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                bat """
                cd c:\\
                echo "xxx"
                """
            }
        }
    }
}
