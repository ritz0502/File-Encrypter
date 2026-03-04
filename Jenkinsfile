pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/ritz0502/File-Encrypter.git'
            }
        }

        stage('Build') {
            steps {
                sh '''
                echo "Building Java project..."
                echo "Listing workspace contents:"
                ls
                cd "Password Protection"
                mkdir -p build
                javac -d build src/*.java
                echo "Build successful"
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                echo "Running tests..."
                cd "Password Protection"
                echo "No automated tests configured"
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploy stage (simulation)"
                echo "Application ready for deployment"
                '''
            }
        }

    }
}
