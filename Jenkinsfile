pipeline {
    agent any 

    options {
        timeout(time: 5, unit: 'MINUTES') 
    }

    stages {
        stage('Run Dynamic Container') {
            steps {
                // 1. Print out the exact phrase requested by your homework assignment
                sh "echo 'this is the main branch'"
                
                // 2. Manually launch a background container and make it hold open for 120 seconds
                // This guarantees it will show up when you run 'docker ps'
                sh "docker run -d --name hw-test-container-${BUILD_NUMBER} ubuntu:latest sleep 120"
            }
        }
    }
}
