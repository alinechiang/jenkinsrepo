pipeline {
    agent any // This tells Jenkins to use any available agent to run the pipeline

    stages {
        stage('Clone repository') {
            steps {
                git 'https://github.com/alinechiang/jenkinsrepo' 
            }
        }

        stage('Run script') {
            steps {
                // Assuming you have a script named 'build.sh' at the root of your repository
                sh './build.sh'
            }
        }
    }
}
