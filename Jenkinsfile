pipeline {
    agent {
        docker { 
            image 'ubuntu:latest' 
        }
    }
    
    options {
        // This ensures builds don't get stuck forever if something goes wrong
        timeout(time: 5, unit: 'MINUTES') 
    }

    stages {
        stage('DevOps Homework Execution') {
            steps {
                // Print the text required by your assignment instructions
                sh "echo 'this is the main branch'"
                
                // Keep the container alive for 120 seconds so you can catch it with 'docker ps'
                sh "sleep 120"
            }
        }
    }
}
