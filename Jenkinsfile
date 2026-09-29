pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn -B clean package'
            }
        }
    }

    post {
        success {
            archiveArtifacts artifacts: 'target/*.war', fingerprint: true
        }
    }
}
