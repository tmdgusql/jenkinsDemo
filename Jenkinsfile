
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                script {
                   def now = new Date()
                   println now.format("yyyyMMddHHmm", TimeZone.getTimeZone('UTC+9'))
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always {
            echo "pipeline job done!!!!!"
        }
    }
}
