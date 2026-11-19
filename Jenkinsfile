
pipeline {
    agent any

    stages {
        stage('Inspect SCM') {
            steps {
                echo 'Jenkinsfile loaded from Git!'

                sh '''
                    echo "Workspace: $WORKSPACE"
                    pwd
                    ls -la
                    cat README.md
                    git log -1 --oneline
                '''
            }
        }
    }
}
