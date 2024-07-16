pipeline {
    agent any
    tools {
        jdk 'JDK_11'  // Replace with the name of your configured JDK
    }
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
