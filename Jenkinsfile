pipeline{
    agent any
    stages{
        stage('build')
        {
            steps{
                echo "this is running"
                sh './gradlew build ==no=daemon'
                archiveArtifacts artifacts: dist/trainSchedule.zip
            }
        }
    }
}
