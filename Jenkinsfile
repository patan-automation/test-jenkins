pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building for Prod environment again now"
                // Add build steps here
            }
        }
        stage('Deploy to Prod') {
            steps {
                build job: 'cd-pipeline-jenkins', // Replace with your target pipeline's job name
                      parameters: [
                          string(name: 'GIT_BRANCH', value: 'main') // Replace with desired branch
                      ]
            }
        }
    }
}
