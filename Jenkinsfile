import java.text.SimpleDateFormat

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
                def dateFormat = new SimpleDateFormat("yyyyMMddHHmm")
                def date = new Date()
                def TODAY = dateFormat.format(date)
    
                echo ${TODAY}
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
