pipeline {
    agent any
    stages {
        stage ("clone") {
            steps {
                echo "cloning the code from Github"
            }
        }
        stage ("Deploy") {
            steps {
                echo "Deploy the code"
                sh "sudo cp -r /var/lib/jenkins/workspace/${JOB_NAME}/* /var/www/html/"
            }
        }
    }
}
