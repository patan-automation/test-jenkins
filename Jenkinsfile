pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building for Dev environment"
                // Add build steps here
            }
        }
        stage('Deploy to Dev') {
            steps {
                build job: 'cd-pipeline-jenkins', // Replace with your target pipeline's job name
                      parameters: [
                          string(name: 'GIT_BRANCH', value: 'dev') // Replace with desired branch
                      ]
            }
        }
    }
}
