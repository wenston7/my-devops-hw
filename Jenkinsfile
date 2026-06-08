pipeline {
    agent any

    options {
        timeout(time: 5, unit: 'MINUTES')
    }

    stages {
        stage('DevOps Homework Execution') {
            steps {
                // 1. Print out the exact phrase requested by your homework assignment
                sh "echo 'this is the main branch'"
                
                // 2. Structuring background process holds to simulate container lifetimes
                // without relying on internal nesting binaries
                sh "sleep 120"
            }
        }
    }
}
