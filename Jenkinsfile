pipeline {

    agent { label 'docker-agent' }

    stages {

        stage("Hello") {
            when {
                expression { env.BRANCH_NAME == 'main' } 
            }
            steps {
                    echo 'This is the testing branch'
            }
        }
        stage('Wildcard Branch Check') {
            when {
                branch 'feature/*' 
            }
            steps {
                echo "Running on a feature branch."
            }
        }
    }
}
