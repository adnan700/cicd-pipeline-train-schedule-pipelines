pipeline {
    agent { docker 'maven:3-alpine' } 
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip
            }
        }
    }
}
